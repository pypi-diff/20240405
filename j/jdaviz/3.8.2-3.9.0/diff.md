# Comparing `tmp/jdaviz-3.8.2.tar.gz` & `tmp/jdaviz-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdaviz-3.8.2.tar", last modified: Fri Feb 23 18:50:07 2024, max compression
+gzip compressed data, was "jdaviz-3.9.0.tar", last modified: Fri Apr  5 17:58:48 2024, max compression
```

## Comparing `jdaviz-3.8.2.tar` & `jdaviz-3.9.0.tar`

### file list

```diff
@@ -1,557 +1,580 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.563869 jdaviz-3.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-23 18:49:51.000000 jdaviz-3.8.2/.bandit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-02-23 18:49:51.000000 jdaviz-3.8.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.471869 jdaviz-3.8.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-02-23 18:49:51.000000 jdaviz-3.8.2/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.471869 jdaviz-3.8.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-02-23 18:49:51.000000 jdaviz-3.8.2/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-23 18:49:51.000000 jdaviz-3.8.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-02-23 18:49:51.000000 jdaviz-3.8.2/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-02-23 18:49:51.000000 jdaviz-3.8.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-02-23 18:49:51.000000 jdaviz-3.8.2/.github/labeler.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.471869 jdaviz-3.8.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-02-23 18:49:51.000000 jdaviz-3.8.2/.github/workflows/changelog_check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-02-23 18:49:51.000000 jdaviz-3.8.2/.github/workflows/ci_cron_weekly.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-02-23 18:49:51.000000 jdaviz-3.8.2/.github/workflows/ci_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-02-23 18:49:51.000000 jdaviz-3.8.2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-02-23 18:49:51.000000 jdaviz-3.8.2/.github/workflows/open_actions.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-02-23 18:49:51.000000 jdaviz-3.8.2/.github/workflows/predeps_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-02-23 18:49:51.000000 jdaviz-3.8.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-02-23 18:49:51.000000 jdaviz-3.8.2/.github/workflows/standalone.yml
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-02-23 18:49:51.000000 jdaviz-3.8.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-02-23 18:49:51.000000 jdaviz-3.8.2/.mailmap
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-02-23 18:49:51.000000 jdaviz-3.8.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    57675 2024-02-23 18:49:51.000000 jdaviz-3.8.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-02-23 18:49:51.000000 jdaviz-3.8.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-02-23 18:49:51.000000 jdaviz-3.8.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-02-23 18:49:51.000000 jdaviz-3.8.2/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-23 18:49:51.000000 jdaviz-3.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-02-23 18:50:07.559869 jdaviz-3.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-02-23 18:49:51.000000 jdaviz-3.8.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-23 18:49:51.000000 jdaviz-3.8.2/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-02-23 18:49:51.000000 jdaviz-3.8.2/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.475869 jdaviz-3.8.2/jdaviz/
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/_astropy_init.py
--rw-r--r--   0 runner    (1001) docker     (127)   103510 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/app.py
--rw-r--r--   0 runner    (1001) docker     (127)    13860 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/app.vue
--rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.479869 jdaviz-3.8.2/jdaviz/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/components/docs_link.vue
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/components/external_link.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/components/glue_state_sync_wrapper.vue
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/components/layer_viewer_icon.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/components/number_uncertainty.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/components/play_pause_widget.vue
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/components/plugin_action_button.vue
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/components/plugin_add_results.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/components/plugin_auto_label.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/components/plugin_dataset_select.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/components/plugin_editable_select.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/components/plugin_file_import_select.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/components/plugin_layer_select.vue
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/components/plugin_layer_select_tabs.vue
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/components/plugin_plot.vue
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/components/plugin_popout.vue
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/components/plugin_section_header.vue
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/components/plugin_subset_select.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/components/plugin_table.vue
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/components/plugin_viewer_select.vue
--rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/components/toolbar_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/components/toolbar_nested.vue
--rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/components/tooltip.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/components/tray_plugin.vue
--rw-r--r--   0 runner    (1001) docker     (127)    11989 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/components/viewer_data_select.vue
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/components/viewer_data_select_item.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.479869 jdaviz-3.8.2/jdaviz/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.479869 jdaviz-3.8.2/jdaviz/configs/cubeviz/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/cubeviz.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/cubeviz.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9617 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.483869 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.483869 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/moment_maps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/moment_maps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.483869 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/moment_maps/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/moment_maps/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/moment_maps/tests/test_moment_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)    21916 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.483869 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/slice/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/slice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10335 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/slice/slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/slice/slice.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.483869 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/slice/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/slice/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/slice/tests/test_slice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.483869 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/spectral_extraction/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/spectral_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/spectral_extraction/spectral_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/spectral_extraction/spectral_extraction.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.483869 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/spectral_extraction/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/spectral_extraction/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/spectral_extraction/tests/test_spectral_extraction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.487869 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/tests/test_cubeviz_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/tests/test_data_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/tests/test_data_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/tests/test_export_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/tests/test_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    13330 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.487869 jdaviz-3.8.2/jdaviz/configs/default/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/default.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.487869 jdaviz-3.8.2/jdaviz/configs/default/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.487869 jdaviz-3.8.2/jdaviz/configs/default/plugins/collapse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/collapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/collapse/collapse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/collapse/collapse.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.487869 jdaviz-3.8.2/jdaviz/configs/default/plugins/collapse/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/collapse/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/collapse/tests/test_collapse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.487869 jdaviz-3.8.2/jdaviz/configs/default/plugins/data_tools/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/data_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/data_tools/data_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/data_tools/data_tools.vue
--rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/data_tools/file_chooser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.491869 jdaviz-3.8.2/jdaviz/configs/default/plugins/export_plot/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/export_plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13781 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/export_plot/export_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/export_plot/export_plot.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.491869 jdaviz-3.8.2/jdaviz/configs/default/plugins/gaussian_smooth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/gaussian_smooth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9316 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.491869 jdaviz-3.8.2/jdaviz/configs/default/plugins/gaussian_smooth/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/gaussian_smooth/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/gaussian_smooth/tests/test_gaussian_smooth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.491869 jdaviz-3.8.2/jdaviz/configs/default/plugins/line_lists/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/line_lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/line_lists/line_list_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    36024 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/line_lists/line_lists.py
--rw-r--r--   0 runner    (1001) docker     (127)    15927 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/line_lists/line_lists.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.491869 jdaviz-3.8.2/jdaviz/configs/default/plugins/line_lists/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/line_lists/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/line_lists/tests/test_line_lists.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.491869 jdaviz-3.8.2/jdaviz/configs/default/plugins/markers/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/markers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/markers/markers.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/markers/markers.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.491869 jdaviz-3.8.2/jdaviz/configs/default/plugins/markers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/markers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12873 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/markers/tests/test_markers_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.491869 jdaviz-3.8.2/jdaviz/configs/default/plugins/metadata_viewer/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/metadata_viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.495869 jdaviz-3.8.2/jdaviz/configs/default/plugins/metadata_viewer/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/metadata_viewer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/metadata_viewer/tests/test_metadata_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.495869 jdaviz-3.8.2/jdaviz/configs/default/plugins/model_fitting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/model_fitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14046 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/model_fitting/fitting_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/model_fitting/initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)    44501 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/model_fitting/model_fitting.py
--rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/model_fitting/model_fitting.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.495869 jdaviz-3.8.2/jdaviz/configs/default/plugins/model_fitting/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/model_fitting/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/model_fitting/tests/test_blackbody.py
--rw-r--r--   0 runner    (1001) docker     (127)    16343 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/model_fitting/tests/test_fitting.py
--rw-r--r--   0 runner    (1001) docker     (127)    19508 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/model_fitting/tests/test_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.495869 jdaviz-3.8.2/jdaviz/configs/default/plugins/plot_options/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/plot_options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49334 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/plot_options/plot_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    31976 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/plot_options/plot_options.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.495869 jdaviz-3.8.2/jdaviz/configs/default/plugins/plot_options/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/plot_options/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14343 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/plot_options/tests/test_plot_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.495869 jdaviz-3.8.2/jdaviz/configs/default/plugins/subset_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/subset_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27187 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.499869 jdaviz-3.8.2/jdaviz/configs/default/plugins/subset_plugin/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/subset_plugin/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/subset_plugin/tests/test_subset_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.499869 jdaviz-3.8.2/jdaviz/configs/default/plugins/subset_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/subset_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/subset_tools/subset_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/subset_tools/subset_tools.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.499869 jdaviz-3.8.2/jdaviz/configs/default/plugins/viewer_creator/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/viewer_creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.vue
--rw-r--r--   0 runner    (1001) docker     (127)    14094 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/default/plugins/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.499869 jdaviz-3.8.2/jdaviz/configs/imviz/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20391 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/imviz.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/imviz.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.499869 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.499869 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/aper_phot_simple/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/aper_phot_simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43836 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.503869 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/catalogs/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/catalogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/catalogs/catalogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/catalogs/catalogs.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.503869 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/compass/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/compass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/compass/compass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/compass/compass.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.503869 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/coords_info/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/coords_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26481 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/coords_info/coords_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/coords_info/coords_info.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.503869 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/footprints/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/footprints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/footprints/footprints.py
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/footprints/footprints.vue
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/footprints/preset_regions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.503869 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/image_viewer_creator/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/image_viewer_creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.503869 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/line_profile_xy/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/line_profile_xy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.507869 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/links_control/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/links_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/links_control/links_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/links_control/links_control.vue
--rw-r--r--   0 runner    (1001) docker     (127)    15687 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.507869 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/rotate_canvas/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/rotate_canvas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.507869 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/rotate_canvas/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/rotate_canvas/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/rotate_canvas/tests/test_rotate_canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/plugins/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.511869 jdaviz-3.8.2/jdaviz/configs/imviz/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.511869 jdaviz-3.8.2/jdaviz/configs/imviz/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/tests/data/ds9_annulus_01.reg
--rw-r--r--   0 runner    (1001) docker     (127)   604800 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/tests/data/gauss100_fits_wcs.fits
--rw-r--r--   0 runner    (1001) docker     (127)   155520 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/tests/data/gauss100_fits_wcs_block_reduced.fits
--rw-r--r--   0 runner    (1001) docker     (127)   155520 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/tests/data/gauss100_fits_wcs_block_reduced_rotated.fits
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/tests/data/miri_i2d_lonlat_gwcs.asdf
--rw-r--r--   0 runner    (1001) docker     (127)    15664 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_astrowidgets_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_catalogs.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_compass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_delete_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_footprints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_line_profile_xy.py
--rw-r--r--   0 runner    (1001) docker     (127)    19497 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_linking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_links_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    25853 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_parser_asdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_parser_roman.py
--rw-r--r--   0 runner    (1001) docker     (127)    13332 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23358 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_simple_aper_phot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_subset_centroid.py
--rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_viewer_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_viewers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_wcs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11747 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/imviz/wcs_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.515869 jdaviz-3.8.2/jdaviz/configs/mosviz/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/mosviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38346 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/mosviz/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/mosviz/mosviz.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/mosviz/mosviz.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.515869 jdaviz-3.8.2/jdaviz/configs/mosviz/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/mosviz/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40180 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/mosviz/plugins/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.515869 jdaviz-3.8.2/jdaviz/configs/mosviz/plugins/row_lock/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/mosviz/plugins/row_lock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/mosviz/plugins/row_lock/row_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/mosviz/plugins/row_lock/row_lock.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.515869 jdaviz-3.8.2/jdaviz/configs/mosviz/plugins/slit_overlay/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/mosviz/plugins/slit_overlay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.515869 jdaviz-3.8.2/jdaviz/configs/mosviz/plugins/slit_overlay/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/mosviz/plugins/slit_overlay/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/mosviz/plugins/slit_overlay/tests/test_slit_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/mosviz/plugins/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    19223 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/mosviz/plugins/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.519869 jdaviz-3.8.2/jdaviz/configs/mosviz/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/mosviz/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/mosviz/tests/test_data_loading.py
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/mosviz/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9463 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/mosviz/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/mosviz/tests/test_source_identifier_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/mosviz/tests/test_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.519869 jdaviz-3.8.2/jdaviz/configs/specviz/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13706 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.519869 jdaviz-3.8.2/jdaviz/configs/specviz/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.519869 jdaviz-3.8.2/jdaviz/configs/specviz/plugins/line_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz/plugins/line_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29910 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.519869 jdaviz-3.8.2/jdaviz/configs/specviz/plugins/line_analysis/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz/plugins/line_analysis/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17721 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz/plugins/line_analysis/tests/test_line_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz/plugins/line_analysis/tests/test_lineflux.py
--rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz/plugins/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.519869 jdaviz-3.8.2/jdaviz/configs/specviz/plugins/unit_conversion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz/plugins/unit_conversion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.519869 jdaviz-3.8.2/jdaviz/configs/specviz/plugins/unit_conversion/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz/plugins/unit_conversion/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz/plugins/unit_conversion/tests/test_unit_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.vue
--rw-r--r--   0 runner    (1001) docker     (127)    25259 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz/plugins/viewers.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz/specviz.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz/specviz.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.523869 jdaviz-3.8.2/jdaviz/configs/specviz/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22581 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz/tests/test_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.523869 jdaviz-3.8.2/jdaviz/configs/specviz2d/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz2d/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.523869 jdaviz-3.8.2/jdaviz/configs/specviz2d/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz2d/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz2d/plugins/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.523869 jdaviz-3.8.2/jdaviz/configs/specviz2d/plugins/spectral_extraction/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz2d/plugins/spectral_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44142 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)    16866 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.523869 jdaviz-3.8.2/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/test_spectral_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz2d/specviz2d.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.523869 jdaviz-3.8.2/jdaviz/configs/specviz2d/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz2d/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz2d/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/configs/specviz2d/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11575 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/container.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.527869 jdaviz-3.8.2/jdaviz/core/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21350 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/core/astrowidgets_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/core/custom_traitlets.py
--rw-r--r--   0 runner    (1001) docker     (127)     8780 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/core/data_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/core/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/core/freezable_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    41235 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/core/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/core/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/core/launcher.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/core/linelists.py
--rw-r--r--   0 runner    (1001) docker     (127)    25703 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/core/marks.py
--rw-r--r--   0 runner    (1001) docker     (127)    14497 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/core/region_translators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/core/registries.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/core/style_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)   151435 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/core/template_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.531869 jdaviz-3.8.2/jdaviz/core/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/core/tests/test_autoconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/core/tests/test_custom_traitlets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/core/tests/test_data_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/core/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/core/tests/test_region_translators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/core/tests/test_template_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/core/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    17493 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/core/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/core/user_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/core/validunits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.463869 jdaviz-3.8.2/jdaviz/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.539869 jdaviz-3.8.2/jdaviz/data/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/blink.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/checktoradial.svg
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/compass.svg
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/contrast.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/cubeviz_icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/home.svg
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/home_match.svg
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/image.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/imviz_icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/left-east.svg
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/line_select.svg
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/line_select_disabled.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/mosviz_icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/pan.svg
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/pan2.svg
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/pan_x.svg
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/pan_x_match.svg
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/pan_y.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/pan_y_match.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/panzoom_match.svg
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/pixelspectra.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/radialtocheck.svg
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/right-east.svg
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/select_annulus.svg
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/select_circle.svg
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/select_ellipse.svg
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/select_lasso.svg
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/select_single_pixel.svg
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/select_x.svg
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/select_xy.svg
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/select_y.svg
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/slice.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/spectral_range.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/specviz2d_icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/specviz_icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/stretch_bounds.svg
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/tune.svg
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/zoom_back.svg
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/zoom_box.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/zoom_box_match.svg
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/zoom_xrange.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/zoom_xrange_match.svg
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/zoom_yrange.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/icons/zoom_yrange_match.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.543869 jdaviz-3.8.2/jdaviz/data/linelists/
--rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/linelists/Atomic-ISO.csv
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/linelists/Atomic-Ionic.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/linelists/Atomic-Ionic_FineStructure.csv
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/linelists/CO-band-heads.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/linelists/CO.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/linelists/Common_Galactic_2000A-11000A.csv
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/linelists/Common_Galactic_700A-2000A.csv
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/linelists/Common_nebular.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/linelists/Common_stellar.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/linelists/DEV_NOTES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/linelists/H-He.csv
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/linelists/H-Paschen-Brackett.csv
--rw-r--r--   0 runner    (1001) docker     (127)    20639 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/linelists/H2-ISO.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/linelists/H2-alt.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/linelists/H2.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/linelists/HeI-HeII.csv
--rw-r--r--   0 runner    (1001) docker     (127)    21334 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/linelists/JWST_line_list_original.txt
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/linelists/PAH.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/linelists/SDSS-IV.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/linelists/SDSS.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/linelists/UV_linelist_vacuum.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/data/linelists/linelist_metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/jdaviz_cli.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/jdaviz_cli_launcher.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.543869 jdaviz-3.8.2/jdaviz/models/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13731 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/models/physical_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.543869 jdaviz-3.8.2/jdaviz/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/tests/coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/tests/test_data_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/tests/test_plugin_is_active.py
--rw-r--r--   0 runner    (1001) docker     (127)    45938 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/tests/test_subsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/tests/test_user_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/tests/test_viewer_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    12527 2024-02-23 18:49:51.000000 jdaviz-3.8.2/jdaviz/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-23 18:50:07.000000 jdaviz-3.8.2/jdaviz/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.559869 jdaviz-3.8.2/jdaviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-02-23 18:50:07.000000 jdaviz-3.8.2/jdaviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20093 2024-02-23 18:50:07.000000 jdaviz-3.8.2/jdaviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 18:50:07.000000 jdaviz-3.8.2/jdaviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-02-23 18:50:07.000000 jdaviz-3.8.2/jdaviz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 18:50:06.000000 jdaviz-3.8.2/jdaviz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-02-23 18:50:07.000000 jdaviz-3.8.2/jdaviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-23 18:50:07.000000 jdaviz-3.8.2/jdaviz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.547869 jdaviz-3.8.2/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-02-23 18:49:51.000000 jdaviz-3.8.2/licenses/GINGA_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-02-23 18:49:51.000000 jdaviz-3.8.2/licenses/IMEXAM_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-02-23 18:49:51.000000 jdaviz-3.8.2/licenses/IPYFILECHOOSER_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-23 18:49:51.000000 jdaviz-3.8.2/licenses/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-02-23 18:49:51.000000 jdaviz-3.8.2/licenses/TEMPLATE_LICENCE.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.547869 jdaviz-3.8.2/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/CubevizExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    17801 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/ImvizDitheredExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    20170 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/ImvizExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8879 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/MosvizExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/MosvizNIRISSExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/Specviz2dExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/SpecvizExample.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.555869 jdaviz-3.8.2/notebooks/concepts/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/cubeviz_contour_overlay.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/cubeviz_data_interactions.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8783 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/cubeviz_fitting.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/cubeviz_ndarray_gif.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/cubeviz_spectral_fitting.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/cubeviz_spectral_spatial_interactions.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/cubeviz_wfc3ir_ramp.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    13949 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/default_programmatic_viewers_from_blank.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/imviz_advanced_aper_phot.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/imviz_color_display.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/imviz_colorbar_mpl.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15370 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/imviz_compass_mpl.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/imviz_custom_colormap.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/imviz_dithered_gwcs.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/imviz_edit_subset_programmatic.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/imviz_line_profiles.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/imviz_load_3d_slices.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/imviz_load_fits_hdu.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    14417 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/imviz_roman_asdf.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/imviz_simple_aper_phot.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    20908 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/mosviz_concept.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    33356 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/mosviz_generate_photometry.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/mosviz_niriss_parser.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/pypi_metrics.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/specviz_from_list.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    82825 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/specviz_from_splot.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/specviz_glue_unit_conversion.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/specviz_line_lists.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/specviz_minimal.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-02-23 18:49:51.000000 jdaviz-3.8.2/notebooks/concepts/specviz_spectrum_list.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-02-23 18:49:51.000000 jdaviz-3.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 18:50:07.563869 jdaviz-3.8.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     5534 2024-02-23 18:49:51.000000 jdaviz-3.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.467869 jdaviz-3.8.2/share/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.467869 jdaviz-3.8.2/share/jupyter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.467869 jdaviz-3.8.2/share/jupyter/nbconvert/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.467869 jdaviz-3.8.2/share/jupyter/nbconvert/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.555869 jdaviz-3.8.2/share/jupyter/nbconvert/templates/jdaviz-default/
--rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-02-23 18:49:51.000000 jdaviz-3.8.2/share/jupyter/nbconvert/templates/jdaviz-default/ansi.js
--rwxr-xr-x   0 runner    (1001) docker     (127)     3653 2024-02-23 18:49:51.000000 jdaviz-3.8.2/share/jupyter/nbconvert/templates/jdaviz-default/app.html
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-23 18:49:51.000000 jdaviz-3.8.2/share/jupyter/nbconvert/templates/jdaviz-default/conf.json
--rwxr-xr-x   0 runner    (1001) docker     (127)     3265 2024-02-23 18:49:51.000000 jdaviz-3.8.2/share/jupyter/nbconvert/templates/jdaviz-default/index.html.j2
--rwxr-xr-x   0 runner    (1001) docker     (127)     5993 2024-02-23 18:49:51.000000 jdaviz-3.8.2/share/jupyter/nbconvert/templates/jdaviz-default/util.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.467869 jdaviz-3.8.2/share/jupyter/voila/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.467869 jdaviz-3.8.2/share/jupyter/voila/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.555869 jdaviz-3.8.2/share/jupyter/voila/templates/jdaviz-default/
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-02-23 18:49:51.000000 jdaviz-3.8.2/share/jupyter/voila/templates/jdaviz-default/index.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.555869 jdaviz-3.8.2/standalone/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-02-23 18:49:51.000000 jdaviz-3.8.2/standalone/entitlements.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 18:50:07.559869 jdaviz-3.8.2/standalone/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-23 18:49:51.000000 jdaviz-3.8.2/standalone/hooks/hook-asdf.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-23 18:49:51.000000 jdaviz-3.8.2/standalone/hooks/hook-bqplot.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-02-23 18:49:51.000000 jdaviz-3.8.2/standalone/hooks/hook-debugpy.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-23 18:49:51.000000 jdaviz-3.8.2/standalone/hooks/hook-glue.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-23 18:49:51.000000 jdaviz-3.8.2/standalone/hooks/hook-glue_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-23 18:49:51.000000 jdaviz-3.8.2/standalone/hooks/hook-ipypopout.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-23 18:49:51.000000 jdaviz-3.8.2/standalone/hooks/hook-jdaviz.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-02-23 18:49:51.000000 jdaviz-3.8.2/standalone/hooks/hook-jupyter_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-23 18:49:51.000000 jdaviz-3.8.2/standalone/hooks/hook-jupyter_events.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-23 18:49:51.000000 jdaviz-3.8.2/standalone/hooks/hook-jupyter_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-23 18:49:51.000000 jdaviz-3.8.2/standalone/hooks/hook-mistune.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-02-23 18:49:51.000000 jdaviz-3.8.2/standalone/hooks/hook-photutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-23 18:49:51.000000 jdaviz-3.8.2/standalone/hooks/hook-pysiaf.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-02-23 18:49:51.000000 jdaviz-3.8.2/standalone/hooks/hook-regions.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-02-23 18:49:51.000000 jdaviz-3.8.2/standalone/hooks/hook-skimage.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-23 18:49:51.000000 jdaviz-3.8.2/standalone/hooks/hook-specreduce.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-02-23 18:49:51.000000 jdaviz-3.8.2/standalone/jdaviz-cli-entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-02-23 18:49:51.000000 jdaviz-3.8.2/standalone/jdaviz.spec
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-02-23 18:49:51.000000 jdaviz-3.8.2/standalone/test_standalone.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-02-23 18:49:51.000000 jdaviz-3.8.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.491143 jdaviz-3.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.bandit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.415144 jdaviz-3.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.415144 jdaviz-3.9.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.415144 jdaviz-3.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/workflows/changelog_check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/workflows/check_milestone.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/workflows/ci_cron_weekly.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/workflows/open_actions.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/workflows/predeps_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.github/workflows/standalone.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-05 17:58:39.000000 jdaviz-3.9.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    62052 2024-04-05 17:58:39.000000 jdaviz-3.9.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-05 17:58:39.000000 jdaviz-3.9.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-05 17:58:39.000000 jdaviz-3.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-05 17:58:39.000000 jdaviz-3.9.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-05 17:58:39.000000 jdaviz-3.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-04-05 17:58:48.491143 jdaviz-3.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-04-05 17:58:39.000000 jdaviz-3.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-05 17:58:39.000000 jdaviz-3.9.0/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-05 17:58:39.000000 jdaviz-3.9.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.419144 jdaviz-3.9.0/jdaviz/
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/_astropy_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118731 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/app.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.423144 jdaviz-3.9.0/jdaviz/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/docs_link.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/external_link.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/glue_state_sync_wrapper.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/layer_viewer_icon.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/multiselect_toggle.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/number_uncertainty.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/play_pause_widget.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_action_button.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_add_results.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_auto_label.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_dataset_select.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_editable_select.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_file_import_select.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_inline_select.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_inline_select_item.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_layer_select.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_layer_select_tabs.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_plot.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_popout.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_previews_temp_disabled.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_section_header.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_subset_select.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_table.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/plugin_viewer_select.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/toolbar_nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/toolbar_nested.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/tooltip.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/tray_plugin.vue
+-rw-r--r--   0 runner    (1001) docker     (127)    13973 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/viewer_data_select.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     7600 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/components/viewer_data_select_item.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.427144 jdaviz-3.9.0/jdaviz/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.427144 jdaviz-3.9.0/jdaviz/configs/cubeviz/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/cubeviz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/cubeviz.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9907 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.427144 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.427144 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/moment_maps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/moment_maps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14738 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.427144 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/moment_maps/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/moment_maps/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10298 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/moment_maps/tests/test_moment_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21916 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.427144 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/slice/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/slice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/slice/slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/slice/slice.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.427144 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/slice/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/slice/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/slice/tests/test_slice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.427144 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/spectral_extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/spectral_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23868 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/spectral_extraction/spectral_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10597 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/spectral_extraction/spectral_extraction.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.427144 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/spectral_extraction/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/spectral_extraction/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16836 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/spectral_extraction/tests/test_spectral_extraction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.431144 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_cubeviz_aperphot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_cubeviz_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_data_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_data_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_export_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16929 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.431144 jdaviz-3.9.0/jdaviz/configs/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/default.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.431144 jdaviz-3.9.0/jdaviz/configs/default/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.431144 jdaviz-3.9.0/jdaviz/configs/default/plugins/collapse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/collapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/collapse/collapse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/collapse/collapse.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.431144 jdaviz-3.9.0/jdaviz/configs/default/plugins/collapse/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/collapse/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/collapse/tests/test_collapse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.431144 jdaviz-3.9.0/jdaviz/configs/default/plugins/data_quality/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/data_quality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/data_quality/dq_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.431144 jdaviz-3.9.0/jdaviz/configs/default/plugins/data_quality/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/data_quality/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/data_quality/tests/test_data_quality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.431144 jdaviz-3.9.0/jdaviz/configs/default/plugins/data_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/data_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/data_tools/data_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/data_tools/data_tools.vue
+-rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/data_tools/file_chooser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.435144 jdaviz-3.9.0/jdaviz/configs/default/plugins/export/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28350 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/export/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10572 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/export/export.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.435144 jdaviz-3.9.0/jdaviz/configs/default/plugins/export/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12441 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/export/tests/test_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.435144 jdaviz-3.9.0/jdaviz/configs/default/plugins/gaussian_smooth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/gaussian_smooth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9436 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.435144 jdaviz-3.9.0/jdaviz/configs/default/plugins/gaussian_smooth/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/gaussian_smooth/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/gaussian_smooth/tests/test_gaussian_smooth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.435144 jdaviz-3.9.0/jdaviz/configs/default/plugins/line_lists/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/line_lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/line_lists/line_list_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36176 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/line_lists/line_lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15989 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/line_lists/line_lists.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.435144 jdaviz-3.9.0/jdaviz/configs/default/plugins/line_lists/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/line_lists/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/line_lists/tests/test_line_lists.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.435144 jdaviz-3.9.0/jdaviz/configs/default/plugins/markers/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/markers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/markers/markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/markers/markers.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.435144 jdaviz-3.9.0/jdaviz/configs/default/plugins/markers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/markers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/markers/tests/test_markers_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.435144 jdaviz-3.9.0/jdaviz/configs/default/plugins/metadata_viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/metadata_viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.439144 jdaviz-3.9.0/jdaviz/configs/default/plugins/metadata_viewer/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/metadata_viewer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/metadata_viewer/tests/test_metadata_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.439144 jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14046 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/fitting_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44501 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/model_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/model_fitting.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.439144 jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/tests/test_blackbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16343 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/tests/test_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19486 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.439144 jdaviz-3.9.0/jdaviz/configs/default/plugins/plot_options/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/plot_options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59261 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/plot_options/plot_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38152 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/plot_options/plot_options.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.439144 jdaviz-3.9.0/jdaviz/configs/default/plugins/plot_options/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/plot_options/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15827 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/plot_options/tests/test_plot_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.439144 jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30851 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.439144 jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_plugin/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_plugin/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8909 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_plugin/tests/test_subset_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_plugin/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.443144 jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_tools/subset_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_tools/subset_tools.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.443144 jdaviz-3.9.0/jdaviz/configs/default/plugins/viewer_creator/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/viewer_creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.vue
+-rw-r--r--   0 runner    (1001) docker     (127)    15412 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/default/plugins/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.443144 jdaviz-3.9.0/jdaviz/configs/imviz/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16990 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/imviz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/imviz.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.443144 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.443144 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/aper_phot_simple/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/aper_phot_simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46898 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.443144 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/catalogs/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/catalogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10293 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/catalogs/catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/catalogs/catalogs.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.443144 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/compass/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/compass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/compass/compass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/compass/compass.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.447144 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/coords_info/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/coords_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26887 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/coords_info/coords_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/coords_info/coords_info.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.447144 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/footprints/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/footprints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25455 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/footprints/footprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/footprints/footprints.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/footprints/preset_regions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.447144 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/image_viewer_creator/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/image_viewer_creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.447144 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/line_profile_xy/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/line_profile_xy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.447144 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/orientation/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/orientation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32344 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/orientation/orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/orientation/orientation.vue
+-rw-r--r--   0 runner    (1001) docker     (127)    16874 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.447144 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/rotate_canvas/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/rotate_canvas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.447144 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/rotate_canvas/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/rotate_canvas/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/rotate_canvas/tests/test_rotate_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16085 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/plugins/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.451144 jdaviz-3.9.0/jdaviz/configs/imviz/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.455144 jdaviz-3.9.0/jdaviz/configs/imviz/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/data/ds9_annulus_01.reg
+-rw-r--r--   0 runner    (1001) docker     (127)   604800 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/data/gauss100_fits_wcs.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   155520 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/data/gauss100_fits_wcs_block_reduced.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   155520 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/data/gauss100_fits_wcs_block_reduced_rotated.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/data/miri_i2d_lonlat_gwcs.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)    15780 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_astrowidgets_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7993 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_compass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_delete_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_footprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_line_profile_xy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_linking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10531 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26072 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_parser_asdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_parser_roman.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13332 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23873 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_simple_aper_phot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_subset_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_viewer_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_viewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7531 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_wcs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20574 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/imviz/wcs_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.455144 jdaviz-3.9.0/jdaviz/configs/mosviz/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38346 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/mosviz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/mosviz.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.455144 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40180 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.455144 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/row_lock/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/row_lock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/row_lock/row_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/row_lock/row_lock.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.455144 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/slit_overlay/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/slit_overlay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.455144 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/slit_overlay/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/slit_overlay/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/slit_overlay/tests/test_slit_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19272 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.455144 jdaviz-3.9.0/jdaviz/configs/mosviz/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/tests/test_data_loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9463 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/tests/test_source_identifier_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/mosviz/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.459143 jdaviz-3.9.0/jdaviz/configs/specviz/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13706 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.459143 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.459143 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/line_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/line_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22575 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7697 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.459143 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/line_analysis/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/line_analysis/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17666 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/line_analysis/tests/test_line_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/line_analysis/tests/test_lineflux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.459143 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/unit_conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/unit_conversion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.459143 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/unit_conversion/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/unit_conversion/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/unit_conversion/tests/test_unit_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.vue
+-rw-r--r--   0 runner    (1001) docker     (127)    26312 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/plugins/viewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/specviz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/specviz.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.459143 jdaviz-3.9.0/jdaviz/configs/specviz/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22581 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz/tests/test_viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.459143 jdaviz-3.9.0/jdaviz/configs/specviz2d/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz2d/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.459143 jdaviz-3.9.0/jdaviz/configs/specviz2d/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz2d/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz2d/plugins/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.463143 jdaviz-3.9.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44142 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17012 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.463143 jdaviz-3.9.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/test_spectral_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz2d/specviz2d.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.463143 jdaviz-3.9.0/jdaviz/configs/specviz2d/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz2d/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz2d/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/configs/specviz2d/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12759 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/container.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.467143 jdaviz-3.9.0/jdaviz/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23254 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/astrowidgets_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/custom_traitlets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8780 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/data_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11992 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9232 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/freezable_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42995 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/launcher.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/linelists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25783 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/marks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14132 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/region_translators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/style_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)   198067 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/template_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.467143 jdaviz-3.9.0/jdaviz/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/tests/test_autoconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/tests/test_custom_traitlets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/tests/test_data_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/tests/test_region_translators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/tests/test_template_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21790 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/core/validunits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.411144 jdaviz-3.9.0/jdaviz/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.467143 jdaviz-3.9.0/jdaviz/data/data_quality/
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/data_quality/jwst.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/data_quality/roman.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.475143 jdaviz-3.9.0/jdaviz/data/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/blink.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/checktoradial.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/compass.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/contrast.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/cubeviz_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/home.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/home_match.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/image.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/imviz_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/left-east.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/line_select.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/line_select_disabled.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/mosviz_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/pan.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/pan2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/pan_x.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/pan_x_match.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/pan_y.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/pan_y_match.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/panzoom_match.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/pixelspectra.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/radialtocheck.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/right-east.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/select_annulus.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/select_circle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/select_ellipse.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/select_lasso.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/select_single_pixel.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/select_x.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/select_xy.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/select_y.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/slice.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/spectral_range.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/specviz2d_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/specviz_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/stretch_bounds.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/tune.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/zoom_back.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/zoom_box.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/zoom_box_match.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/zoom_xrange.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/zoom_xrange_match.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/zoom_yrange.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/icons/zoom_yrange_match.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.479143 jdaviz-3.9.0/jdaviz/data/linelists/
+-rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/Atomic-ISO.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/Atomic-Ionic.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/Atomic-Ionic_FineStructure.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/CO-band-heads.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/CO.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/Common_Galactic_2000A-11000A.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/Common_Galactic_700A-2000A.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/Common_nebular.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/Common_stellar.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/DEV_NOTES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/H-He.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/H-Paschen-Brackett.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    20639 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/H2-ISO.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/H2-alt.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/H2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/HeI-HeII.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    21334 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/JWST_line_list_original.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/PAH.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/SDSS-IV.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/SDSS.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/UV_linelist_vacuum.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/data/linelists/linelist_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/jdaviz_cli.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/jdaviz_cli_launcher.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/main_styles.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.479143 jdaviz-3.9.0/jdaviz/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13731 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/models/physical_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/style_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.479143 jdaviz-3.9.0/jdaviz/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/tests/coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/tests/test_data_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/tests/test_plugin_is_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48140 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/tests/test_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/tests/test_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/tests/test_viewer_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13463 2024-04-05 17:58:39.000000 jdaviz-3.9.0/jdaviz/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-05 17:58:48.000000 jdaviz-3.9.0/jdaviz/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.491143 jdaviz-3.9.0/jdaviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-04-05 17:58:48.000000 jdaviz-3.9.0/jdaviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20936 2024-04-05 17:58:48.000000 jdaviz-3.9.0/jdaviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:58:48.000000 jdaviz-3.9.0/jdaviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-05 17:58:48.000000 jdaviz-3.9.0/jdaviz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:58:47.000000 jdaviz-3.9.0/jdaviz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-05 17:58:48.000000 jdaviz-3.9.0/jdaviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-05 17:58:48.000000 jdaviz-3.9.0/jdaviz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.479143 jdaviz-3.9.0/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-05 17:58:39.000000 jdaviz-3.9.0/licenses/GINGA_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-05 17:58:39.000000 jdaviz-3.9.0/licenses/IMEXAM_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-05 17:58:39.000000 jdaviz-3.9.0/licenses/IPYFILECHOOSER_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-05 17:58:39.000000 jdaviz-3.9.0/licenses/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-05 17:58:39.000000 jdaviz-3.9.0/licenses/TEMPLATE_LICENCE.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.483143 jdaviz-3.9.0/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/CubevizExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    16821 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/ImvizDitheredExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    19158 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/ImvizExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8879 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/MosvizExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/MosvizNIRISSExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/Specviz2dExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/SpecvizExample.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.487143 jdaviz-3.9.0/notebooks/concepts/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15331 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/cubeviz_aperture_photometry.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/cubeviz_contour_overlay.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/cubeviz_data_interactions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8783 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/cubeviz_fitting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/cubeviz_ndarray_gif.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/cubeviz_spectral_fitting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/cubeviz_spectral_spatial_interactions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/cubeviz_wfc3ir_ramp.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13949 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/default_programmatic_viewers_from_blank.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/imviz_advanced_aper_phot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/imviz_color_display.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/imviz_colorbar_mpl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15370 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/imviz_compass_mpl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/imviz_custom_colormap.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/imviz_dithered_gwcs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/imviz_edit_subset_programmatic.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/imviz_line_profiles.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/imviz_load_3d_slices.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/imviz_load_fits_hdu.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15426 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/imviz_roman_asdf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/imviz_simple_aper_phot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    20908 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/mosviz_concept.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    33356 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/mosviz_generate_photometry.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/mosviz_niriss_parser.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/pypi_metrics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/specviz_from_list.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    82825 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/specviz_from_splot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/specviz_glue_unit_conversion.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/specviz_line_lists.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/specviz_minimal.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-05 17:58:39.000000 jdaviz-3.9.0/notebooks/concepts/specviz_spectrum_list.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-05 17:58:39.000000 jdaviz-3.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 17:58:48.491143 jdaviz-3.9.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5534 2024-04-05 17:58:39.000000 jdaviz-3.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.411144 jdaviz-3.9.0/share/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.411144 jdaviz-3.9.0/share/jupyter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.411144 jdaviz-3.9.0/share/jupyter/nbconvert/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.411144 jdaviz-3.9.0/share/jupyter/nbconvert/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.487143 jdaviz-3.9.0/share/jupyter/nbconvert/templates/jdaviz-default/
+-rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-04-05 17:58:39.000000 jdaviz-3.9.0/share/jupyter/nbconvert/templates/jdaviz-default/ansi.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3653 2024-04-05 17:58:39.000000 jdaviz-3.9.0/share/jupyter/nbconvert/templates/jdaviz-default/app.html
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 17:58:39.000000 jdaviz-3.9.0/share/jupyter/nbconvert/templates/jdaviz-default/conf.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3265 2024-04-05 17:58:39.000000 jdaviz-3.9.0/share/jupyter/nbconvert/templates/jdaviz-default/index.html.j2
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5993 2024-04-05 17:58:39.000000 jdaviz-3.9.0/share/jupyter/nbconvert/templates/jdaviz-default/util.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.411144 jdaviz-3.9.0/share/jupyter/voila/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.411144 jdaviz-3.9.0/share/jupyter/voila/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.487143 jdaviz-3.9.0/share/jupyter/voila/templates/jdaviz-default/
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-05 17:58:39.000000 jdaviz-3.9.0/share/jupyter/voila/templates/jdaviz-default/index.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.487143 jdaviz-3.9.0/standalone/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/entitlements.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:58:48.491143 jdaviz-3.9.0/standalone/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-asdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-bqplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-debugpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-glue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-glue_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-ipypopout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-jdaviz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-jupyter_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-jupyter_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-jupyter_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-mistune.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-photutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-pysiaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-skimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/hooks/hook-specreduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/jdaviz-cli-entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/jdaviz.spec
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-05 17:58:39.000000 jdaviz-3.9.0/standalone/test_standalone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-05 17:58:39.000000 jdaviz-3.9.0/tox.ini
```

### Comparing `jdaviz-3.8.2/.github/ISSUE_TEMPLATE/bug_report.yaml` & `jdaviz-3.9.0/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/.github/ISSUE_TEMPLATE/feature_request.yaml` & `jdaviz-3.9.0/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/.github/PULL_REQUEST_TEMPLATE.md` & `jdaviz-3.9.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files 9% similar despite different names*

```diff
@@ -34,9 +34,9 @@
 
 - [ ] Are two approvals required? Branch protection rule does not check for the second approval. If a second approval is not necessary, please apply the `trivial` label.
 - [ ] Do the proposed changes actually accomplish desired goals? Also manually run the affected example notebooks, if necessary.
 - [ ] Do the proposed changes follow the [STScI Style Guides](https://github.com/spacetelescope/style-guides)?
 - [ ] Are tests added/updated as required? If so, do they follow the [STScI Style Guides](https://github.com/spacetelescope/style-guides)?
 - [ ] Are docs added/updated as required? If so, do they follow the [STScI Style Guides](https://github.com/spacetelescope/style-guides)?
 - [ ] Did the CI pass? If not, are the failures related?
-- [ ] Is a milestone set? Set this to bugfix milestone if this is a bug fix and needs to be released ASAP; otherwise, set this to the next major release milestone.
+- [ ] Is a milestone set? Set this to bugfix milestone if this is a bug fix and needs to be released ASAP; otherwise, set this to the next major release milestone. Bugfix milestone also needs an accompanying backport label.
 - [ ] After merge, any internal documentations need updating (e.g., JIRA, Innerspace)?
```

### Comparing `jdaviz-3.8.2/.github/workflows/ci_cron_weekly.yml` & `jdaviz-3.9.0/.github/workflows/ci_cron_weekly.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/.github/workflows/ci_workflows.yml` & `jdaviz-3.9.0/.github/workflows/ci_workflows.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/.github/workflows/codeql-analysis.yml` & `jdaviz-3.9.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/.github/workflows/predeps_workflows.yml` & `jdaviz-3.9.0/.github/workflows/predeps_workflows.yml`

 * *Files 10% similar despite different names*

```diff
@@ -16,32 +16,33 @@
 jobs:
   # Github Actions supports ubuntu, windows, and macos virtual environments:
   # https://help.github.com/en/actions/reference/virtual-environments-for-github-hosted-runners
   ci_tests:
     name: ${{ matrix.name }}
     runs-on: ${{ matrix.os }}
     strategy:
+      fail-fast: false
       matrix:
         include:
 
           - name: RC testing on Linux with remote data
             os: ubuntu-latest
-            python: '3.11'
-            toxenv: py311-test-predeps
+            python: '3.12'
+            toxenv: py312-test-predeps
             toxposargs: --remote-data
 
           - name: RC testing on OSX
             os: macos-latest
             python: 3.9
             toxenv: py39-test-predeps
 
           - name: RC testing on Windows
             os: windows-latest
-            python: '3.10'
-            toxenv: py310-test-predeps
+            python: '3.11'
+            toxenv: py311-test-predeps
 
     steps:
     - name: Checkout code
       uses: actions/checkout@v4
       with:
         fetch-depth: 0
     - name: Set up python ${{ matrix.python }} on ${{ matrix.os }}
```

### Comparing `jdaviz-3.8.2/.github/workflows/publish.yml` & `jdaviz-3.9.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/.github/workflows/standalone.yml` & `jdaviz-3.9.0/.github/workflows/standalone.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/.gitignore` & `jdaviz-3.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/.mailmap` & `jdaviz-3.9.0/.mailmap`

 * *Files 3% similar despite different names*

```diff
@@ -20,7 +20,8 @@
 Nicholas Earl <contact@nicholasearl.me> <nearl@stsci.edu>
 Nicholas Earl <contact@nicholasearl.me> nmearl <contact@nicholasearl.me>
 Ori Fox <ofox@stsci.edu> Ori <ofox@stsci.edu>
 P. L. Lim <2090236+pllim@users.noreply.github.com>
 Patrick Ogle <pogle@stsci.edu> PatrickOgle <pogle@stsci.edu>
 Ricky O'Steen <39831871+rosteen@users.noreply.github.com> <rosteen@stsci.edu>
 Ricky O'Steen <39831871+rosteen@users.noreply.github.com> rosteen <39831871+rosteen@users.noreply.github.com>
+Gilbert Green <42986583+gibsongreen@users.noreply.github.com> <ggreen@tapangalia2023.local>
```

### Comparing `jdaviz-3.8.2/.readthedocs.yaml` & `jdaviz-3.9.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/CHANGES.rst` & `jdaviz-3.9.0/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,130 @@
+3.9 (2024-04-05)
+================
+
+New Features
+------------
+- Stretch bounds tool now enables dynamic adjustment of spline knots. [#2545, #2623]
+
+- Stretch histogram shows a spinner when the histogram data is updating. [#2644]
+
+- Spectrum and image viewer bounds can now be set through the Plot Options UI. [#2604, #2649]
+
+- Opacity for spatial subsets is now adjustable from within Plot Options. [#2663]
+
+- Live-preview of aperture selection in plugins. [#2664, #2684]
+
+- "Export Plot" plugin is now replaced with the more general "Export" plugin. [#2722, #2782]
+
+- "Export" plugin supports exporting plugin tables, plugin plots, data, and
+  non-composite spatial subsets.[#2755, #2774, #2760, #2772, #2770, #2780, #2784]
+
+- Opening a plugin in the tray (from the API or the toolbar buttons) now scrolls to that plugin.
+  [#2768]
+
+Cubeviz
+^^^^^^^
+
+- Calculated moments can now be output in velocity units. [#2584, #2588, #2665, #2697]
+
+- Added functionality to Collapse and Spectral Extraction plugins to save results to FITS file. [#2586]
+
+- Moment map plugin now supports linear per-spaxel continuum subtraction. [#2587]
+
+- Single-pixel subset tool now shows spectrum-at-spaxel on hover. [#2647]
+
+- Spectral extraction plugin re-organized into subsections to be more consistent with specviz2d. [#2676]
+
+- Add conical aperture support to cubeviz in the spectral extraction plugin. [#2679]
+
+- New aperture photometry plugin that can perform aperture photometry on selected cube slice. [#2666]
+
+- Live previews in spectral extraction plugin. [#2733]
+
+- Slice plugin is refactored to rely on the spectral value instead of the slice index.  This removes
+  both the slider and slice-index input. [#2715]
+
+Imviz
+^^^^^
+
+- There is now option for image rotation in Orientation (was Links Control) plugin.
+  This feature requires WCS linking. [#2179, #2673, #2699, #2734, #2759]
+
+- Add "Random" colormap for visualizing image segmentation maps. [#2671]
+
+- Enabling any matched zoom tool in a viewer disables other matched zoom tools in other viewers
+  to avoid recursion. [#2764]
+
+Specviz2d
+^^^^^^^^^
+
+- Spectral extraction plugin: highlighting of active header section. [#2676]
+
+API Changes
+-----------
+
+- ``width`` argument in Line Analysis plugin is renamed to ``continuum_width`` and ``width``
+  will be removed in a future release. [#2587]
+
+- New API access to ``viz.data_labels``, ``viewer.data_labels_visible``, and
+  ``viewer.data_labels_loaded``. [#2626]
+
+Cubeviz
+^^^^^^^
+
+- ``spatial_subset`` in the spectral extraction plugin is now renamed to ``aperture`` and the deprecated name will
+  be removed in a future release. [#2664]
+
+- Slice plugin's ``wavelength``, ``wavelength_unit``, and ``show_wavelength`` are deprecated in favor
+  of ``value``, ``value_unit``, and ``show_value``, respectively.  ``slice`` is also deprecated
+  and should be replaced with accessing/setting ``value`` directly. [#2706, #2715]
+
+- Disabled exporting spectrum-viewer to PNG in Cubeviz; pending investigation/bugfix. [#2777]
+
+Imviz
+^^^^^
+
+- Links Control plugin is now called Orientation. [#2179]
+
+- Linking by WCS will now always generate a hidden reference data layer
+  without distortion. As a result, when WCS linked, the first loaded data
+  is no longer the reference data. Additionally, if data is distorted,
+  its distortion will show when linked by WCS. If there is also data without WCS,
+  it can no longer be displayed when WCS linked. [#2179]
+
+- ``imviz.link_data()`` inputs and behaviors are now consistent with the Orientation plugin. [#2179]
+
+- Single-pixel tool is no longer available. To mark a single-pixel area, use Markers plugin. [#2710]
+
+Bug Fixes
+---------
+
+- Fix redshifted line lists that were displaying at rest wavelengths, by assuming a global redshift. [#2726]
+
+- Order of RGB preset colors now matches for less than and greater than 5 layers. [#2731]
+
+Cubeviz
+^^^^^^^
+
+- Spectral extraction now ignores NaNs. [#2737]
+
+Imviz
+^^^^^
+
+- Apertures that are selected and later modified to be invalid properly show a warning. [#2684]
+
+- Histogram in Plot Options no longer stalls for a very large image. [#2735]
+
+Specviz
+^^^^^^^
+
+- Check unit type (e.g., flux density, surface brightness, counts, etc) for generating
+  display label for the y axis in spectral viewer. Previously it was hard coded
+  to always display ``flux density`` no matter the input unit. [#2703]
+
 3.8.2 (2024-02-23)
 ==================
 
 Bug Fixes
 ---------
 
 * Fix app top-bar alignment in popouts and when embedded in websites. [#2648]
@@ -49,14 +172,15 @@
 - Fixes viewer keys in ``viz.viewers`` for additionally created viewers. [#2624]
 
 Specviz
 ^^^^^^^
 
 -  Fixed parser bug where an HDUList would load as SpectrumList, even though it was a Spectrum1D. [#2576]
 
+
 3.8 (2023-11-29)
 ================
 
 New Features
 ------------
 
 - Plots in plugins now include basic zoom/pan tools for Plot Options,
```

### Comparing `jdaviz-3.8.2/CITATION.cff` & `jdaviz-3.9.0/CITATION.cff`

 * *Files 2% similar despite different names*

```diff
@@ -69,13 +69,13 @@
   orcid: "https://orcid.org/0009-0008-4112-7418"
 - family-names: "Tollerud"
   given-names: "Erik"
   orcid: "https://orcid.org/0000-0002-9599-310X"
 - family-names: "Volfman"
   given-names: "Sabrina"
 title: "Jdaviz"
-version: 3.8.2
+version: 3.9.0
 doi: https://doi.org/10.5281/zenodo.5513927
-date-released: 2024-02-23
+date-released: 2024-04-05
 url: "https://github.com/spacetelescope/jdaviz"
 
 # see a full list of contributors here: https://github.com/spacetelescope/jdaviz/graphs/contributors
```

### Comparing `jdaviz-3.8.2/CODE_OF_CONDUCT.md` & `jdaviz-3.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/LICENSE.rst` & `jdaviz-3.9.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/PKG-INFO` & `jdaviz-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdaviz
-Version: 3.8.2
+Version: 3.9.0
 Summary: Astronomical data analysis development leveraging the Jupyter platform
 Author-email: JDADF Developers <help@stsci.edu>
 Project-URL: Homepage, https://jdaviz.readthedocs.io/en/latest/
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 Requires-Dist: packaging
```

### Comparing `jdaviz-3.8.2/README.rst` & `jdaviz-3.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/conftest.py` & `jdaviz-3.9.0/conftest.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/__init__.py` & `jdaviz-3.9.0/jdaviz/__init__.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/_astropy_init.py` & `jdaviz-3.9.0/jdaviz/_astropy_init.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/app.py` & `jdaviz-3.9.0/jdaviz/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,60 @@
+import operator
 import os
 import pathlib
 import re
 import uuid
 import warnings
-import operator
-
-from ipywidgets import widget_serialization
 import ipyvue
-
 from astropy import units as u
 from astropy.nddata import NDData
 from astropy.io import fits
 from astropy.time import Time
 from echo import CallbackProperty, DictCallbackProperty, ListCallbackProperty
 from ipygoldenlayout import GoldenLayout
 from ipysplitpanes import SplitPanes
-from traitlets import Dict, Bool, Unicode, Any
-from specutils import Spectrum1D, SpectralRegion
 import matplotlib.cm as cm
 import numpy as np
-
-from glue.config import colormaps
-from glue.config import settings as glue_settings
+from glue.config import colormaps, settings as glue_settings
 from glue.core import HubListener
 from glue.core.link_helpers import LinkSame, LinkSameWithUnits
 from glue.core.message import (DataCollectionAddMessage,
                                DataCollectionDeleteMessage,
                                SubsetCreateMessage,
                                SubsetUpdateMessage,
                                SubsetDeleteMessage)
+from glue.core.roi import CircularROI, CircularAnnulusROI, EllipticalROI, RectangularROI
 from glue.core.state_objects import State
 from glue.core.subset import (RangeSubsetState, RoiSubsetState,
                               CompositeSubsetState, InvertState)
-from glue.core.roi import CircularROI, CircularAnnulusROI, EllipticalROI, RectangularROI
 from glue.core.units import unit_converter
 from glue_astronomy.spectral_coordinates import SpectralCoordinates
 from glue_astronomy.translators.regions import roi_subset_state_to_region
 from glue_jupyter.app import JupyterApplication
 from glue_jupyter.common.toolbar_vuetify import read_icon
-from glue_jupyter.bqplot.common.tools import TrueCircularROI
 from glue_jupyter.state_traitlets_helpers import GlueState
+from ipypopout import PopoutButton
 from ipyvuetify import VuetifyTemplate
+from ipywidgets import widget_serialization
+from traitlets import Dict, Bool, Unicode, Any
+from specutils import Spectrum1D, SpectralRegion
 
 from jdaviz import __version__
+from jdaviz import style_registry
 from jdaviz.core.config import read_configuration, get_configuration
 from jdaviz.core.events import (LoadDataMessage, NewViewerMessage, AddDataMessage,
                                 SnackbarMessage, RemoveDataMessage,
                                 AddDataToViewerMessage, RemoveDataFromViewerMessage,
                                 ViewerAddedMessage, ViewerRemovedMessage,
-                                ViewerRenamedMessage)
-from jdaviz.core.style_widget import StyleWidget
+                                ViewerRenamedMessage, ChangeRefDataMessage)
 from jdaviz.core.registries import (tool_registry, tray_registry, viewer_registry,
                                     data_parser_registry)
 from jdaviz.core.tools import ICON_DIR
-from jdaviz.utils import SnackbarQueue, alpha_index, MultiMaskSubsetState
-from ipypopout import PopoutButton
+from jdaviz.utils import (SnackbarQueue, alpha_index, data_has_valid_wcs, layer_is_table_data,
+                          MultiMaskSubsetState, _wcs_only_label)
 
 __all__ = ['Application', 'ALL_JDAVIZ_CONFIGS']
 
 SplitPanes()
 GoldenLayout()
 
 CONTAINER_TYPES = dict(row='gl-row', col='gl-col', stack='gl-stack')
@@ -126,21 +122,25 @@
                      'j-viewer-data-select-item': 'components/viewer_data_select_item.vue',
                      'j-layer-viewer-icon': 'components/layer_viewer_icon.vue',
                      'j-tray-plugin': 'components/tray_plugin.vue',
                      'j-play-pause-widget': 'components/play_pause_widget.vue',
                      'j-plugin-section-header': 'components/plugin_section_header.vue',
                      'j-number-uncertainty': 'components/number_uncertainty.vue',
                      'j-plugin-popout': 'components/plugin_popout.vue',
+                     'j-multiselect-toggle': 'components/multiselect_toggle.vue',
+                     'plugin-previews-temp-disabled': 'components/plugin_previews_temp_disabled.vue',  # noqa
                      'plugin-table': 'components/plugin_table.vue',
                      'plugin-dataset-select': 'components/plugin_dataset_select.vue',
                      'plugin-subset-select': 'components/plugin_subset_select.vue',
                      'plugin-viewer-select': 'components/plugin_viewer_select.vue',
                      'plugin-layer-select': 'components/plugin_layer_select.vue',
                      'plugin-layer-select-tabs': 'components/plugin_layer_select_tabs.vue',
                      'plugin-editable-select': 'components/plugin_editable_select.vue',
+                     'plugin-inline-select': 'components/plugin_inline_select.vue',
+                     'plugin-inline-select-item': 'components/plugin_inline_select_item.vue',
                      'plugin-action-button': 'components/plugin_action_button.vue',
                      'plugin-add-results': 'components/plugin_add_results.vue',
                      'plugin-auto-label': 'components/plugin_auto_label.vue',
                      'plugin-file-import-select': 'components/plugin_file_import_select.vue',
                      'glue-state-sync-wrapper': 'components/glue_state_sync_wrapper.vue'}
 
 _verbosity_levels = ('debug', 'info', 'warning', 'error')
@@ -150,14 +150,17 @@
 for name, path in custom_components.items():
     ipyvue.register_component_from_file(None, name,
                                         os.path.join(os.path.dirname(__file__), path))
 
 ipyvue.register_component_from_file('g-viewer-tab', "container.vue", __file__)
 
 
+style_registry.add((__file__, 'main_styles.vue'))
+
+
 class ApplicationState(State):
     """
     The application state object contains all the current front-end state,
     including the loaded data name references, the active viewers, plugins,
     and layout.
 
     This state object allows for nested callbacks in mutable objects like
@@ -202,15 +205,17 @@
         },
         'layout': {
         }
     }, docstring="Top-level application settings.")
 
     icons = DictCallbackProperty({
         'radialtocheck': read_icon(os.path.join(ICON_DIR, 'radialtocheck.svg'), 'svg+xml'),
-        'checktoradial': read_icon(os.path.join(ICON_DIR, 'checktoradial.svg'), 'svg+xml')
+        'checktoradial': read_icon(os.path.join(ICON_DIR, 'checktoradial.svg'), 'svg+xml'),
+        'nuer': read_icon(os.path.join(ICON_DIR, 'right-east.svg'), 'svg+xml'),
+        'nuel': read_icon(os.path.join(ICON_DIR, 'left-east.svg'), 'svg+xml')
     }, docstring="Custom application icons")
 
     viewer_icons = DictCallbackProperty({}, docstring="Indexed icons (numbers) for viewers across the app")  # noqa
     layer_icons = DictCallbackProperty({}, docstring="Indexed icons (letters) for layers across the app")  # noqa
 
     data_items = ListCallbackProperty(
         docstring="List of data items parsed from the Glue data collection.")
@@ -248,21 +253,23 @@
     template_file = __file__, "app.vue"
 
     loading = Bool(False).tag(sync=True)
     config = Unicode("").tag(sync=True)
     vdocs = Unicode("").tag(sync=True)
     docs_link = Unicode("").tag(sync=True)
     popout_button = Any().tag(sync=True, **widget_serialization)
+    style_registry_instance = Any().tag(sync=True, **widget_serialization)
 
     def __init__(self, configuration=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._jdaviz_helper = None
         self._verbosity = 'warning'
         self._history_verbosity = 'info'
         self.popout_button = PopoutButton(self)
+        self.style_registry_instance = style_registry.get_style_registry()
 
         # Generate a state object for this application to maintain the state of
         #  the user interface.
         self.state = ApplicationState()
 
         # The application handler stores the state of the data and the
         #  underlying glue infrastructure
@@ -290,21 +297,34 @@
                    ['Reversed: Magma', cm.magma_r],
                    ['Reversed: Hot', cm.hot_r],
                    ['Reversed: Rainbow', cm.rainbow_r])
         for cur_cm in new_cms:
             if cur_cm not in colormaps.members:
                 colormaps.add(*cur_cm)
 
+        from jdaviz.core.events import PluginTableAddedMessage, PluginPlotAddedMessage
+        self._plugin_tables = {}
+        self.hub.subscribe(self, PluginTableAddedMessage,
+                           handler=self._on_plugin_table_added)
+        self._plugin_plots = {}
+        self.hub.subscribe(self, PluginPlotAddedMessage,
+                           handler=self._on_plugin_plot_added)
+
         # Parse the yaml configuration file used to compose the front-end UI
         self.load_configuration(configuration)
 
         # If true, link data on load. If false, do not link data to speed up
         # data loading
         self.auto_link = kwargs.pop('auto_link', True)
 
+        # Imviz linking
+        self._link_type = 'pixels'
+        if self.config == "imviz":
+            self._wcs_use_affine = None
+
         # Subscribe to messages indicating that a new viewer needs to be
         #  created. When received, information is passed to the application
         #  handler to generate the appropriate viewer instance.
         self.hub.subscribe(self, NewViewerMessage,
                            handler=self._on_new_viewer)
 
         # Subscribe to messages indicating new data should be loaded into the
@@ -340,24 +360,41 @@
 
         # Internal cache so we don't have to keep calling get_object for the same Data.
         # Key should be (data_label, statistic) and value the translated object.
         self._get_object_cache = {}
         self.hub.subscribe(self, SubsetUpdateMessage,
                            handler=lambda msg: self._clear_object_cache(msg.subset.label))
 
+        # Store for associations between Data entries:
+        self._data_associations = self._init_data_associations()
+
         # Subscribe to messages that result in changes to the layers
         self.hub.subscribe(self, AddDataMessage,
                            handler=self._on_layers_changed)
         self.hub.subscribe(self, RemoveDataMessage,
                            handler=self._on_layers_changed)
         self.hub.subscribe(self, SubsetCreateMessage,
                            handler=self._on_layers_changed)
         self.hub.subscribe(self, SubsetDeleteMessage,
                            handler=self._on_layers_changed)
 
+    def _on_plugin_table_added(self, msg):
+        if msg.plugin._plugin_name is None:
+            # plugin was instantiated after the app was created, ignore
+            return
+        key = f"{msg.plugin._plugin_name}: {msg.table._table_name}"
+        self._plugin_tables.setdefault(key, msg.table.user_api)
+
+    def _on_plugin_plot_added(self, msg):
+        if msg.plugin._plugin_name is None:
+            # plugin was instantiated after the app was created, ignore
+            return
+        key = f"{msg.plugin._plugin_name}: {msg.plot._plot_name}"
+        self._plugin_plots.setdefault(key, msg.plot.user_api)
+
     @property
     def hub(self):
         """
         Reference to the stored application handler `~glue.core.hub.Hub` instance
         for the application.
         """
         return self._application_handler.data_collection.hub
@@ -403,27 +440,26 @@
 
     @history_verbosity.setter
     def history_verbosity(self, val):
         if val not in _verbosity_levels:
             raise ValueError(f'Invalid verbosity: {val}')
         self._history_verbosity = val
 
-    def set_style_template_file(self, path):
+    def _add_style(self, path):
         """
-        Sets the path to a vue file containing a <style> tag that will be applied on top of the
-        style defined in ``app.vue``.  This is useful for config-specific or downstream styling
-        at the app-level.
+        Appends an addition vue file containing a <style> tag that will be applied on top of the
+        style defined in ``main_styles.vue``.  This is useful for config-specific or downstream
+        styling at the app-level.
 
         Parameters
         ----------
         path : str or tuple
             Path to a ``.vue`` file containing style rules to inject into the app.
         """
-        style_widget = StyleWidget(path)
-        self.state.style_widget = "IPY_MODEL_" + style_widget.model_id
+        style_registry.add(path)
 
     def _on_snackbar_message(self, msg):
         """
         Displays a toast message with an editable message that be dismissed
         manually or will dismiss automatically after a timeout.
 
         Whether the message shows as a snackbar popup is controlled by ``self.verbosity``,
@@ -457,22 +493,129 @@
         self.state.snackbar_queue.put(self.state, msg,
                                       history=msg_level >= history_level,
                                       popup=msg_level >= popup_level)
 
     def _on_layers_changed(self, msg):
         if hasattr(msg, 'data'):
             layer_name = msg.data.label
+            is_wcs_only = msg.data.meta.get(_wcs_only_label, False)
+            is_not_child = self._get_assoc_data_parent(layer_name) is None
+            children_layers = self._get_assoc_data_children(layer_name)
+
         elif hasattr(msg, 'subset'):
             layer_name = msg.subset.label
+            is_wcs_only = False
+            is_not_child = True
+            children_layers = []
         else:
             raise NotImplementedError(f"cannot recognize new layer from {msg}")
 
+        wcs_only_refdata_icon = ''  # blank - might be replaced with custom icon in the future
+        # any changes here should also be manually reflected in orientation.vue
+        orientation_icons = {'Default orientation': 'mdi-image-outline',
+                             'North-up, East-left': 'nuel',
+                             'North-up, East-right': 'nuer'}
+
         if layer_name not in self.state.layer_icons:
-            self.state.layer_icons = {**self.state.layer_icons,
-                                      layer_name: alpha_index(len(self.state.layer_icons))}
+            if is_wcs_only:
+                self.state.layer_icons = {**self.state.layer_icons,
+                                          layer_name: orientation_icons.get(layer_name,
+                                                                            wcs_only_refdata_icon)}
+            elif is_not_child:
+                self.state.layer_icons = {
+                    **self.state.layer_icons,
+                    layer_name: alpha_index(len([ln for ln, ic in self.state.layer_icons.items()
+                                                 if not ic.startswith('mdi-') and
+                                                 self._get_assoc_data_parent(ln) is None]))
+                }
+
+        # all remaining layers at this point have a parent:
+        child_layer_icons = {}
+        for layer_name in self.state.layer_icons:
+            children_layers = self._get_assoc_data_children(layer_name)
+            if children_layers is not None:
+                parent_icon = self.state.layer_icons[layer_name]
+                for i, child_layer in enumerate(children_layers, start=1):
+                    child_layer_icons[child_layer] = f'{parent_icon}{i}'
+
+        self.state.layer_icons = {
+            **self.state.layer_icons,
+            **child_layer_icons
+        }
+
+    def _change_reference_data(self, new_refdata_label, viewer_id=None):
+        """
+        Change reference data to Data with ``data_label``.
+        This does not work on data without WCS.
+        """
+        if self.config != 'imviz':
+            # this method is only meant for Imviz for now
+            return
+
+        if viewer_id is None:
+            viewer = self._jdaviz_helper.default_viewer._obj
+        else:
+            viewer = self.get_viewer(viewer_id)
+
+        old_refdata = viewer.state.reference_data
+
+        if old_refdata is not None and ((new_refdata_label == old_refdata.label)
+                                        or (old_refdata.coords is None)):
+            # if there's no refdata change nor WCS, don't do anything:
+            return
+
+        if old_refdata is None:
+            return
+
+        # locate the central coordinate of old refdata in this viewer:
+        sky_cen = viewer._get_center_skycoord()
+
+        # estimate FOV in the viewer with old reference data:
+        fov_sky_init = viewer._get_fov()
+
+        new_refdata = self.data_collection[new_refdata_label]
+
+        # make sure new refdata can be selected:
+        refdata_choices = [choice.label for choice in viewer.state.ref_data_helper.choices]
+        if new_refdata_label not in refdata_choices:
+            viewer.state.ref_data_helper.append_data(new_refdata)
+        viewer.state.ref_data_helper.refresh()
+
+        # set the new reference data in the viewer:
+        viewer.state.reference_data = new_refdata
+
+        # also update the viewer item's reference data label:
+        viewer_ref = viewer.reference
+        viewer_item = self._get_viewer_item(viewer_ref)
+        viewer_item['reference_data_label'] = new_refdata.label
+
+        self.hub.broadcast(ChangeRefDataMessage(
+            new_refdata,
+            viewer,
+            viewer_id=viewer.reference,
+            old=old_refdata,
+            sender=self))
+
+        if (
+            all('_WCS_ONLY' in refdata.meta for refdata in [old_refdata, new_refdata]) and
+            viewer.shape is not None
+        ):
+            # adjust zoom to account for new refdata if both the
+            # old and new refdata are WCS-only layers
+            # (which also ensures zoom_level is already determined):
+            fov_sky_final = viewer._get_fov()
+            viewer.zoom(
+                float(fov_sky_final / fov_sky_init)
+            )
+
+        # only re-center the viewer if all data layers have WCS:
+        has_wcs_per_data = [data_has_valid_wcs(d) for d in viewer.data()]
+        if all(has_wcs_per_data):
+            # re-center the viewer on previous location.
+            viewer.center_on(sky_cen)
 
     def _link_new_data(self, reference_data=None, data_to_be_linked=None):
         """
         When additional data is loaded, check to see if the spectral axis of
         any components are compatible with already loaded data. If so, link
         them so that they can be displayed on the same profile1D plot.
         """
@@ -673,14 +816,25 @@
 
     def get_viewer_by_id(self, vid):
         """Like :meth:`get_viewer` but use ID directly instead of reference name.
         This is useful when reference name is `None`.
         """
         return self._viewer_store.get(vid)
 
+    def _get_wcs_from_subset(self, subset_state):
+        """ Usually WCS is subset.parent.coords, except special cubeviz case."""
+
+        if self.config == 'cubeviz':
+            parent_data = subset_state.attributes[0].parent
+            wcs = parent_data.meta.get("_orig_spatial_wcs", None)
+        else:
+            wcs = subset_state.xatt.parent.coords
+
+        return wcs
+
     def get_subsets(self, subset_name=None, spectral_only=False,
                     spatial_only=False, object_only=False,
                     simplify_spectral=True, use_display_units=False,
                     include_sky_region=False):
         """
         Returns all branches of glue subset tree in the form that subset plugin
         can recognize.
@@ -729,15 +883,14 @@
                 # Region composed of multiple ROI or Range subset
                 # objects that must be traversed
                 subset_region = self.get_sub_regions(subset.subset_state,
                                                      simplify_spectral, use_display_units,
                                                      get_sky_regions=include_sky_region)
 
             elif isinstance(subset.subset_state, RoiSubsetState):
-
                 subset_region = self._get_roi_subset_definition(subset.subset_state,
                                                                 to_sky=include_sky_region)
 
             elif isinstance(subset.subset_state, RangeSubsetState):
                 # 2D regions represented as SpectralRegion objects
                 subset_region = self._get_range_subset_bounds(subset.subset_state,
                                                               simplify_spectral,
@@ -861,19 +1014,15 @@
     def _get_roi_subset_definition(self, subset_state, to_sky=False):
 
         # pixel region
         roi_as_region = roi_subset_state_to_region(subset_state)
 
         wcs = None
         if to_sky:
-            if self.config == 'cubeviz':
-                parent_data = subset_state.attributes[0].parent
-                wcs = parent_data.meta.get("_orig_spatial_wcs", None)
-            else:
-                wcs = subset_state.xatt.parent.coords  # imviz, try getting WCS from subset data
+            wcs = self._get_wcs_from_subset(subset_state)
 
         # if no spatial wcs on subset, we have to skip computing sky region for this subset
         # but want to do so without raising an error (since many subsets could be requested)
         roi_as_sky_region = None
         if wcs is not None:
             roi_as_sky_region = roi_as_region.to_sky(wcs)
 
@@ -1143,43 +1292,62 @@
             if new_state is None:
                 new_state = convert_to_range
             else:
                 new_state = new_state | convert_to_range
 
         return new_state
 
-    def add_data(self, data, data_label=None, notify_done=True):
+    def add_data(self, data, data_label=None, notify_done=True, parent=None):
         """
         Add data to the Glue ``DataCollection``.
 
         Parameters
         ----------
         data : any
             Data to be stored in the ``DataCollection``. This must either be
             a `~glue.core.data.Data` instance, or an arbitrary data instance
             for which there exists data translation functions in the
             glue astronomy repository.
         data_label : str, optional
             The name associated with this data. If none is given, label is pulled
             from the input data (if `~glue.core.data.Data`) or a generic name is
             generated.
-        notify_done: bool
+        notify_done : bool
             Flag controlling whether a snackbar message is set when the data is
             added to the app. Set to False to avoid overwhelming the user if
             lots of data is getting loaded at once.
+        parent : str, optional
+            Associate the added Data entry as the child of layer ``parent``.
         """
 
         if not data_label and hasattr(data, "label"):
             data_label = data.label
         data_label = self.return_unique_name(data_label)
         if data_label in self.data_collection.labels:
             warnings.warn(f"Overwriting existing data entry with label '{data_label}'")
 
         self.data_collection[data_label] = data
 
+        # manage associated Data entries:
+        self._add_assoc_data_as_parent(data_label)
+        if parent is not None:
+            data_collection_labels = [data.label for data in self.data_collection]
+            if parent not in data_collection_labels:
+                raise ValueError(f'parent "{parent}" is not a valid data label in '
+                                 f'the data collection: {data_collection_labels}.')
+
+            # Does the parent Data have a parent? If so, raise error:
+            parent_of_parent = self._get_assoc_data_parent(parent)
+            if parent_of_parent is not None:
+                raise NotImplementedError('Data associations are currently supported '
+                                          'between root layers (without parents) and their '
+                                          f'children, but the proposed parent "{parent}" has '
+                                          f'parent "{parent_of_parent}".')
+            self._set_assoc_data_as_child(data_label, new_parent_label=parent)
+
         # Send out a toast message
         if notify_done:
             snackbar_message = SnackbarMessage(
                 f"Data '{data_label}' successfully added.", sender=self, color="success")
             self.hub.broadcast(snackbar_message)
 
     def return_data_label(self, loaded_object, ext=None, alt_name=None, check_unique=True):
@@ -1658,14 +1826,15 @@
             The item from the data collection off of which to move the subset definitions.
 
         new_parent : glue.core.Data, str
             The item from the data collection to make the new parent. If None, the first
             item in the data collection that doesn't match ``old_parent`` will be chosen.
         '''
         from astropy.wcs.utils import pixel_to_pixel
+        from jdaviz.configs.imviz.wcs_utils import get_compass_info
 
         if isinstance(old_parent, str):
             old_parent = self.data_collection[old_parent]
 
         if isinstance(new_parent, str):
             new_parent = self.data_collection[new_parent]
         elif new_parent is None:
@@ -1690,20 +1859,31 @@
                             data_components = new_parent.components
                             if subset_att not in data_components:
                                 cid = [c for c in data_components if c.label == subset_att.label][0]
                                 setattr(subset_state, att, cid)
 
                     # Translate bounds through WCS if needed
                     if (self.config == "imviz" and
-                            self._jdaviz_helper.plugins["Links Control"].link_type == "WCS"):
+                            self._jdaviz_helper.plugins["Orientation"].link_type == "WCS"):
+
+                        # Default shape for WCS-only layers is 10x10, but it doesn't really matter
+                        # since we only need the angles.
+                        old_angle, _, old_flip = get_compass_info(old_parent.coords, (10, 10))[-3:]
+                        new_angle, _, new_flip = get_compass_info(new_parent.coords, (10, 10))[-3:]
+                        if old_flip != new_flip:
+                            # Note that this won't work for an irregular/assymetric region if we
+                            # ever implement those.
+                            relative_angle = 180 - new_angle - old_angle
+                        else:
+                            relative_angle = new_angle - old_angle
+
                         # Get the correct link to use for translation
                         roi = subset_state.roi
-                        if type(roi) in (CircularROI, CircularAnnulusROI,
-                                         EllipticalROI, TrueCircularROI):
-                            old_xc, old_yc = subset_state.center()
+                        old_xc, old_yc = subset_state.center()
+                        if isinstance(roi, (CircularROI, CircularAnnulusROI, EllipticalROI)):
                             # Convert center
                             x, y = pixel_to_pixel(old_parent.coords, new_parent.coords,
                                                   roi.xc, roi.yc)
                             subset_state.move_to(x, y)
 
                             for att in ("radius", "inner_radius", "outer_radius",
                                         "radius_x", "radius_y"):
@@ -1711,28 +1891,47 @@
                                 # Do we need to worry about using x for the radius conversion for
                                 # radius_y if there is distortion?
                                 r = getattr(roi, att, None)
                                 if r is not None:
                                     dummy_x = old_xc + r
                                     x2, y2 = pixel_to_pixel(old_parent.coords, new_parent.coords,
                                                             dummy_x, old_yc)
-                                    new_radius = np.abs(x2 - x)
+                                    # Need to use x and y in this radius calculation because the
+                                    # new orientation is likely rotated compared to the original.
+                                    new_radius = np.sqrt((x2 - x)**2 + (y2 - y)**2)
                                     setattr(roi, att, new_radius)
 
-                        elif type(roi) is RectangularROI:
-                            x_min, y_min = pixel_to_pixel(old_parent.coords, new_parent.coords,
-                                                          roi.xmin, roi.ymin)
-                            x_max, y_max = pixel_to_pixel(old_parent.coords, new_parent.coords,
-                                                          roi.xmax, roi.ymax)
-                            roi.xmin = x_min
-                            roi.xmax = x_max
-                            roi.ymin = y_min
-                            roi.ymax = y_max
+                        elif isinstance(roi, RectangularROI):
+                            x1, y1 = pixel_to_pixel(old_parent.coords, new_parent.coords,
+                                                    roi.xmin, roi.ymin)
+                            x2, y2 = pixel_to_pixel(old_parent.coords, new_parent.coords,
+                                                    roi.xmin, roi.ymax)
+                            x3, y3 = pixel_to_pixel(old_parent.coords, new_parent.coords,
+                                                    roi.xmax, roi.ymin)
+
+                            # Calculate new width and height from possibly rotated result
+                            new_half_width = np.sqrt((x3-x1)**2 + (y3-y1)**2) * 0.5
+                            new_half_height = np.sqrt((x2-x1)**2 + (y2-y1)**2) * 0.5
+
+                            # Convert center
+                            new_center = pixel_to_pixel(old_parent.coords, new_parent.coords,
+                                                        old_xc, old_yc)
+
+                            # New min/max before applying theta
+                            roi.xmin = new_center[0] - new_half_width
+                            roi.xmax = new_center[0] + new_half_width
+                            roi.ymin = new_center[1] - new_half_height
+                            roi.ymax = new_center[1] + new_half_height
+
+                        # Account for rotation between orientations
+                        if hasattr(roi, "theta"):
+                            fac = 1.0 if (old_flip != new_flip) else -1.0
+                            roi.theta = (fac * (np.deg2rad(relative_angle) - roi.theta)) % (2 * np.pi)  # noqa: E501
 
-                    elif type(subset_group.subset_state) is RangeSubsetState:
+                    elif isinstance(subset_group.subset_state, RangeSubsetState):
                         range_state = subset_group.subset_state
                         cur_unit = old_parent.coords.spectral_axis.unit
                         new_unit = new_parent.coords.spectral_axis.unit
                         if cur_unit is not new_unit:
                             range_state.lo, range_state.hi = cur_unit.to(new_unit, [range_state.lo,
                                                                                     range_state.hi])
 
@@ -1784,29 +1983,35 @@
         self.remove_data_from_viewer(event['id'], data_label)
 
     def vue_data_item_visibility(self, event):
         self.set_data_visibility(event['id'],
                                  self._get_data_item_by_id(event['item_id'])['name'],
                                  visible=event['visible'], replace=event.get('replace', False))
 
+    def vue_change_reference_data(self, event):
+        self._change_reference_data(
+            self._get_data_item_by_id(event['item_id'])['name'],
+            viewer_id=self._get_viewer_item(event['id'])['name']
+        )
+
     def set_data_visibility(self, viewer_reference, data_label, visible=True, replace=False):
         """
         Set the visibility of the layers corresponding to ``data_label`` in a given viewer.
 
         Parameters
         ----------
         viewer_reference : str
             Reference (or ID) of the viewer
         data_label : str
             Label of the data to set the visiblity.  If not already loaded in the viewer, the
             data will automatically be loaded before setting the visibility
         visible : bool
             Whether to set the layer(s) to visible.
         replace : bool
-            Whether to disable the visilility of all other layers in the viewer
+            Whether to disable the visibility of all other layers in the viewer
         """
         viewer_item = self._get_viewer_item(viewer_reference)
         viewer_id = viewer_item['id']
         viewer = self.get_viewer_by_id(viewer_id)
 
         # if the data_label is in the app, but not loaded in the viewer, automatically load it first
         viewer_data_labels = [layer.layer.label for layer in viewer.layers]
@@ -1835,77 +2040,105 @@
             add_data_message = AddDataMessage(data, viewer,
                                               viewer_id=viewer_id,
                                               sender=self)
             self.hub.broadcast(add_data_message)
 
         # set visibility state of all applicable layers
         for layer in viewer.layers:
+            layer_is_wcs_only = getattr(layer.layer, 'meta', {}).get(_wcs_only_label, False)
             if layer.layer.data.label == data_label:
-                if visible and not layer.visible:
+                if layer_is_wcs_only:
+                    layer.visible = False
+                    layer.update()
+                elif visible and not layer.visible:
                     layer.visible = True
                     layer.update()
                 else:
                     layer.visible = visible
 
         # if replace, do another loop (we do a second loop to ensure the visible layer is added
         # first BEFORE other layers are removed)
         if replace:
             for layer in viewer.layers:
                 if layer.layer.data.label != data_label:
                     layer.visible = False
 
+        # if Data has children, update their visibilities to match Data:
+        assoc_children = self._get_assoc_data_children(data_label)
+        for layer in viewer.layers:
+            for data_label in assoc_children:
+                if layer.layer.data.label == data_label:
+                    if visible and not layer.visible:
+                        layer.visible = True
+                        layer.update()
+                    else:
+                        layer.visible = visible
+
         # update data menu - selected_data_items should be READ ONLY, not modified by the user/UI
         selected_items = viewer_item['selected_data_items']
         data_id = self._data_id_from_label(data_label)
         selected_items[data_id] = 'visible' if visible else 'hidden'
         if replace:
             for id in selected_items:
                 if id != data_id:
                     selected_items[id] = 'hidden'
 
+        # remove WCS-only data from selected items, add to wcs_only_layers:
+        for layer in viewer.layers:
+            layer_is_wcs_only = getattr(layer.layer, 'meta', {}).get(_wcs_only_label, False)
+            if layer.layer.data.label == data_label and layer_is_wcs_only:
+                layer.visible = False
+                if data_label not in viewer.state.wcs_only_layers:
+                    viewer.state.wcs_only_layers.append(data_label)
+                selected_items.pop(data_id)
+
         # Sets the plot axes labels to be the units of the most recently
         # active data.
         viewer_data_labels = [layer.layer.label for layer in viewer.layers]
         if len(viewer_data_labels) > 0 and getattr(self._jdaviz_helper, '_in_batch_load', 0) == 0:
             # This "if" is nested on purpose to make parent "if" available
             # for other configs in the future, as needed.
             if self.config == 'imviz':
                 viewer.on_limits_change()  # Trigger compass redraw
 
     def vue_data_item_remove(self, event):
 
         data_label = event['item_name']
         data = self.data_collection[data_label]
-        self._reparent_subsets(data)
+        orientation_plugin = self._jdaviz_helper.plugins.get("Orientation")
+        if orientation_plugin is not None:
+            from jdaviz.configs.imviz.plugins.orientation.orientation import base_wcs_layer_label
+            orient = orientation_plugin.orientation.selected
+            if orient == data_label:
+                orient = base_wcs_layer_label
+            self._reparent_subsets(data, new_parent=orient)
+        else:
+            self._reparent_subsets(data)
 
-        # Make sure the data isn't loaded in any viewers
-        for viewer_id in self._viewer_store:
+        # Make sure the data isn't loaded in any viewers and isn't the selected orientation
+        for viewer_id, viewer in self._viewer_store.items():
+            if orientation_plugin is not None and self._link_type == 'wcs':
+                if viewer.state.reference_data.label == data_label:
+                    self._change_reference_data(base_wcs_layer_label, viewer_id)
             self.remove_data_from_viewer(viewer_id, data_label)
 
-        # Imviz has some extra logic below that can be skipped after data removal if we're not
-        # removing the reference data, so we check that here.
-        if self.config == "imviz":
-            imviz_refdata = False
-            ref_data, iref = self._jdaviz_helper.get_ref_data()
-            if data is ref_data:
-                imviz_refdata = True
-
         self.data_collection.remove(self.data_collection[data_label])
 
-        # If there are two or more datasets left we need to link them back together after removing
-        # the reference data (which would leave 0 external_links).
-        if len(self.data_collection) > 1 and len(self.data_collection.external_links) == 0:
-            if self.config == "imviz" and imviz_refdata:
-                link_type = self._jdaviz_helper.plugins["Links Control"].link_type.selected.lower()
-                self._jdaviz_helper.link_data(link_type=link_type, error_on_fail=True)
+        # If there are two or more datasets left we need to link them back together if anything
+        # was linked only through the removed data.
+        if (len(self.data_collection) > 1 and
+                len(self.data_collection.external_links) < len(self.data_collection) - 1):
+            if orientation_plugin is not None:
+                orientation_plugin._obj._link_image_data()
                 # Hack to restore responsiveness to imviz layers
                 for viewer_ref in self.get_viewer_reference_names():
                     viewer = self.get_viewer(viewer_ref)
                     loaded_layers = [layer.layer.label for layer in viewer.layers if
-                                     "Subset" not in layer.layer.label]
+                                     "Subset" not in layer.layer.label and layer.layer.label
+                                     not in orientation_plugin.orientation.labels]
                     if len(loaded_layers):
                         self.remove_data_from_viewer(viewer_ref, loaded_layers[-1])
                         self.add_data_to_viewer(viewer_ref, loaded_layers[-1])
             else:
                 for i in range(1, len(self.data_collection)):
                     self._link_new_data(data_to_be_linked=i)
 
@@ -1975,19 +2208,23 @@
             viewer._check_if_data_removed(msg=msg)
 
         self._clear_object_cache(msg.data.label)
 
     def _create_data_item(self, data):
         ndims = len(data.shape)
         wcsaxes = data.meta.get('WCSAXES', None)
+        wcs_only = data.meta.get(_wcs_only_label, False)
         if wcsaxes is None:
             # then we'll need to determine type another way, we want to avoid
             # this when we can though since its not as cheap
             component_ids = [str(c) for c in data.component_ids()]
-        if data.label == 'MOS Table':
+
+        if wcs_only:
+            typ = 'wcs-only'
+        elif data.label == 'MOS Table':
             typ = 'table'
         elif 'Trace' in data.meta:
             typ = 'trace'
         elif ndims == 1:
             typ = '1d spectrum'
         elif ndims == 2 and wcsaxes is not None:
             if wcsaxes == 3:
@@ -2024,14 +2261,16 @@
 
         return {
             'id': str(uuid.uuid4()),
             'name': data.label,
             'locked': False,
             'ndims': data.ndim,
             'type': typ,
+            'has_wcs': data_has_valid_wcs(data),
+            'is_astrowidgets_markers_table': (self.config == "imviz") and layer_is_table_data(data),
             'meta': {k: v for k, v in data.meta.items() if _expose_meta(k)},
             'children': []}
 
     @staticmethod
     def _create_stack_item(container='gl-stack', children=None, viewers=None):
         """
         Convenience method for generating stack item dictionaries.
@@ -2068,15 +2307,16 @@
             return 0
 
         # Assume name-num format
         last_vid = all_vids[-1]
         last_num = int(last_vid.split('-')[-1])
         return last_num + 1
 
-    def _create_viewer_item(self, viewer, vid=None, name=None, reference=None):
+    def _create_viewer_item(self, viewer, vid=None, name=None, reference=None,
+                            open_data_menu_if_empty=True):
         """
         Convenience method for generating viewer item dictionaries.
 
         Parameters
         ----------
         viewer : `~glue_jupyter.bqplot.common.BqplotBaseView`
             The ``Bqplot`` viewer instance.
@@ -2084,15 +2324,17 @@
             The ID of the viewer.
         name : str or `None`, optional
             The name shown in the GoldenLayout tab for this viewer.
             If `None`, it is the same as viewer ID.
         reference : str, optional
             The reference associated with this viewer as defined in the yaml
             configuration file.
-
+        open_data_menu_if_empty : bool, optional
+            Whether the data menu should be opened when creating the viewer if the viewer is
+            empty.  Pass this as False if immediately populating the viewer.
         Returns
         -------
         dict
             Dictionary containing information for this viewer item.
         """
         if vid is None:
             pfx = self.state.settings.get('configuration', str(name))
@@ -2102,30 +2344,42 @@
         # There is a viewer.LABEL inherited from glue-jupyter but there was
         # objection in using it here because it is not hidden, so we use our
         # own attribute instead.
         viewer._reference_id = vid  # For reverse look-up
 
         self.state.viewer_icons.setdefault(vid, len(self.state.viewer_icons)+1)
 
+        wcs_only_layers = getattr(viewer.state, 'wcs_only_layers', [])
+
+        reference_data = getattr(viewer.state, 'reference_data', None)
+        reference_data_label = getattr(reference_data, 'label', None)
+        linked_by_wcs = getattr(viewer.state, 'linked_by_wcs', False)
+
         return {
             'id': vid,
             'name': name or vid,
             'widget': "IPY_MODEL_" + viewer.figure_widget.model_id,
             'toolbar': "IPY_MODEL_" + viewer.toolbar.model_id if viewer.toolbar else '',  # noqa
             'layer_options': "IPY_MODEL_" + viewer.layer_options.model_id,
             'viewer_options': "IPY_MODEL_" + viewer.viewer_options.model_id,
             'selected_data_items': {},  # noqa data_id: visibility state (visible, hidden, mixed), READ-ONLY
             'visible_layers': {},  # label: {color, label_suffix}, READ-ONLY
+            'wcs_only_layers': wcs_only_layers,
+            'reference_data_label': reference_data_label,
             'canvas_angle': 0,  # canvas rotation clockwise rotation angle in deg
             'canvas_flip_horizontal': False,  # canvas rotation horizontal flip
             'config': self.config,  # give viewer access to app config/layout
             'collapse': True,
-            'reference': reference}
+            'reference': reference or name or vid,
+            'linked_by_wcs': linked_by_wcs,
+            'open_data_menu_if_empty': open_data_menu_if_empty  # noqa open menu on init if viewer is empty
+        }
 
-    def _on_new_viewer(self, msg, vid=None, name=None):
+    def _on_new_viewer(self, msg, vid=None, name=None, add_layers_to_viewer=False,
+                       open_data_menu_if_empty=True):
         """
         Callback for when the `~jdaviz.core.events.NewViewerMessage` message is
         raised. This method asks the application handler to generate a new
         viewer and then created the associated stack and viewer items.
 
         Parameters
         ----------
@@ -2136,60 +2390,90 @@
             ID of the viewer. If `None`, it is auto-generated
             from configuration settings.
 
         name : str or `None`
             Name of the viewer. If `None`, it is auto-generated
             from class name.
 
+        open_data_menu_if_empty : bool, optional
+            Whether the data menu should be opened when creating the viewer if the viewer is
+            empty.  Pass this as False if immediately populating the viewer.
+
         Returns
         -------
         viewer : `~glue_jupyter.bqplot.common.BqplotBaseView`
             The new viewer instance.
         """
+
         viewer = self._application_handler.new_data_viewer(
             msg.cls, data=msg.data, show=False)
         viewer.figure_widget.layout.height = '100%'
 
+        linked_by_wcs = self._link_type == 'wcs'
+
         if hasattr(viewer.state, 'linked_by_wcs'):
-            links_control_plugin = self._jdaviz_helper.plugins.get('Links Control', None)
-            if links_control_plugin is not None:
-                viewer.state.linked_by_wcs = links_control_plugin.link_type.selected == 'WCS'
-            elif len(self._viewer_store):
+            orientation_plugin = self._jdaviz_helper.plugins.get('Orientation', None)
+            if orientation_plugin is not None:
+                linked_by_wcs = orientation_plugin.link_type.selected == 'WCS'
+            elif len(self._viewer_store) and hasattr(self._jdaviz_helper, 'default_viewer'):
                 # The plugin would only not exist for instances of Imviz where the user has
-                # intentionally removed the Links Control plugin, but in that case we will
+                # intentionally removed the Orientation plugin, but in that case we will
                 # adopt "linked_by_wcs" from the first (assuming all are the same)
                 # NOTE: deleting the default viewer is forbidden both by API and UI, but if
                 # for some reason that was the case here, linked_by_wcs will default to False
-                viewer.state.linked_by_wcs = list(self._viewer_store.values())[0].state.linked_by_wcs  # noqa
+                linked_by_wcs = self._jdaviz_helper.default_viewer._obj.state.linked_by_wcs
+            else:
+                linked_by_wcs = False
+            viewer.state.linked_by_wcs = linked_by_wcs
+
+        if linked_by_wcs:
+            from jdaviz.configs.imviz.helper import get_wcs_only_layer_labels
+            viewer.state.wcs_only_layers = get_wcs_only_layer_labels(self)
 
         if msg.x_attr is not None:
             x = msg.data.id[msg.x_attr]
             viewer.state.x_att = x
 
         # Create the viewer item dictionary
         if name is None:
             name = vid
         new_viewer_item = self._create_viewer_item(
-            viewer=viewer, vid=vid, name=name, reference=name
+            viewer=viewer, vid=vid, name=name, reference=name,
+            open_data_menu_if_empty=open_data_menu_if_empty
         )
 
+        if self.config == 'imviz':
+            # NOTE: if ever extending image rotation beyond imviz or adding non-image viewers
+            # to imviz: this currently assumes that the helper has a default_viewer and that is an
+            # image viewer
+            ref_data = self._jdaviz_helper.default_viewer._obj.state.reference_data
+            new_viewer_item['reference_data_label'] = getattr(ref_data, 'label', None)
+
+            if hasattr(viewer, 'reference'):
+                viewer.state.reference_data = ref_data
+
         new_stack_item = self._create_stack_item(
             container='gl-stack',
             viewers=[new_viewer_item])
 
         # Store the glupyter viewer object so we can access the add and remove
         #  data methods in the future
         vid = new_viewer_item['id']
         self._viewer_store[vid] = viewer
 
         # Add viewer locally
         self.state.stack_items.append(new_stack_item)
 
         self.session.application.viewers.append(viewer)
 
+        if add_layers_to_viewer:
+            for layer_label in add_layers_to_viewer:
+                if hasattr(viewer, 'reference'):
+                    self.add_data_to_viewer(viewer.reference, layer_label)
+
         # Send out a toast message
         self.hub.broadcast(ViewerAddedMessage(vid, sender=self))
 
         return viewer
 
     def load_configuration(self, path=None, config=None):
         """
@@ -2300,25 +2584,27 @@
                 )
 
                 if opt_value is None:
                     continue
 
                 optional_tray_kwargs[opt_kwarg] = opt_value
 
-            tray_item_instance = tray.get('cls')(
-                app=self, **optional_tray_kwargs
-            )
             # store a copy of the tray name in the instance so it can be accessed by the
             # plugin itself
             tray_item_label = tray.get('label')
-            tray_item_instance._plugin_name = tray_item_label
 
+            tray_item_instance = tray.get('cls')(
+                app=self, plugin_name=tray_item_label, **optional_tray_kwargs
+            )
+
+            # NOTE: is_relevant is later updated by observing irrelevant_msg traitlet
             self.state.tray_items.append({
                 'name': name,
                 'label': tray_item_label,
+                'is_relevant': len(tray_item_instance.irrelevant_msg) == 0,
                 'widget': "IPY_MODEL_" + tray_item_instance.model_id
             })
 
     def _reset_state(self):
         """ Resets the application state """
         self.state = ApplicationState()
         self._application_handler._tools = {}
@@ -2380,7 +2666,31 @@
                 tray_item = widget_serialization['from_json'](ipy_model_id, None)
                 break
 
         if tray_item is None:
             raise KeyError(f'{name} not found in app.state.tray_items')
 
         return tray_item
+
+    def _init_data_associations(self):
+        # assume all Data are parents:
+        data_associations = {
+            data.label: {'parent': None, 'children': []}
+            for data in self.data_collection
+        }
+        return data_associations
+
+    def _add_assoc_data_as_parent(self, data_label):
+        self._data_associations[data_label] = {'parent': None, 'children': []}
+
+    def _set_assoc_data_as_child(self, data_label, new_parent_label):
+        # Data has a new parent:
+        self._data_associations[data_label]['parent'] = new_parent_label
+        # parent has a new child:
+        self._data_associations[new_parent_label]['children'].append(data_label)
+
+    def _get_assoc_data_children(self, data_label):
+        # intentionally not recursive for now, just one generation:
+        return self._data_associations.get(data_label, {}).get('children', [])
+
+    def _get_assoc_data_parent(self, data_label):
+        return self._data_associations.get(data_label, {}).get('parent')
```

### Comparing `jdaviz-3.8.2/jdaviz/cli.py` & `jdaviz-3.9.0/jdaviz/cli.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/components/docs_link.vue` & `jdaviz-3.9.0/jdaviz/components/docs_link.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/components/glue_state_sync_wrapper.vue` & `jdaviz-3.9.0/jdaviz/components/glue_state_sync_wrapper.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/components/layer_viewer_icon.vue` & `jdaviz-3.9.0/jdaviz/components/layer_viewer_icon.vue`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 <template>
   <span v-if="icon !== undefined">
-    <v-icon v-if="String(icon).startsWith('mdi-')" size="16">
+    <v-icon v-if="String(icon).startsWith('mdi-')" :size="icon_size || 16">
       {{icon}}
     </v-icon>
+    <span v-else-if="icons && Object.keys(icons).indexOf(icon) !== -1">
+      <img :src="icons[icon]" :width="icon_size || 16"/>
+    </span>
     <span v-else :class="prevent_invert_if_dark ? 'layer-viewer-icon' : 'invert-if-dark layer-viewer-icon'" :style="span_style+'; color: '+color+'; '+borderStyle">
       {{String(icon).toUpperCase()}}
     </span>
   </span>
 </template>
 
 <script>
 module.exports = {
-  props: ['span_style', 'color', 'icon', 'linewidth', 'linestyle', 'prevent_invert_if_dark'],
+  props: ['span_style', 'color', 'icon', 'icons', 'icon_size', 'linewidth', 'linestyle', 'prevent_invert_if_dark'],
   computed: {
     borderStyle() {
       if (this.$props.linewidth > 0) { 
         return 'border-bottom: '+this.$props.linewidth+'px '+this.$props.linestyle+' '+this.$props.color
       }
       return ''
     },
```

### Comparing `jdaviz-3.8.2/jdaviz/components/number_uncertainty.vue` & `jdaviz-3.9.0/jdaviz/components/number_uncertainty.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/components/play_pause_widget.vue` & `jdaviz-3.9.0/jdaviz/components/play_pause_widget.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/components/plugin_add_results.vue` & `jdaviz-3.9.0/jdaviz/components/plugin_add_results.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/components/plugin_auto_label.vue` & `jdaviz-3.9.0/jdaviz/components/plugin_auto_label.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/components/plugin_dataset_select.vue` & `jdaviz-3.9.0/jdaviz/components/plugin_dataset_select.vue`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
       </template>
    </v-select>
   </v-row>
  </div>
 </template>
 <script>
 module.exports = {
-  props: ['items', 'selected', 'label', 'hint', 'rules', 'show_if_single_entry', 'multiselect']
+  props: ['items', 'selected', 'label', 'hint', 'rules', 'show_if_single_entry', 'multiselect'],
 };
 </script>
 
 <style scoped>
   .v-select__selections {
     flex-wrap: nowrap !important;
     display: block !important;
```

### Comparing `jdaviz-3.8.2/jdaviz/components/plugin_editable_select.vue` & `jdaviz-3.9.0/jdaviz/components/plugin_editable_select.vue`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
           <v-icon style="cursor: pointer" @click="modeAdd">mdi-plus</v-icon>
         </j-tooltip>
       </template>
     </v-select>
     <v-alert
       v-else-if="mode=='remove'"
       type="warning"
-      style="width: 100%"
+      style="width: 100%; padding-top: 16px; padding-bottom: 16px"
     >
       <span>remove '{{selected}}' {{label.toLowerCase()}}?</span>
       <template v-slot:append>
         <j-tooltip tooltipcontent="cancel">
           <v-icon style="cursor: pointer" @click="changeCancel">mdi-close</v-icon>
         </j-tooltip>
         <j-tooltip :tooltipcontent="'Remove '+selected+' '+label.toLowerCase()">
```

### Comparing `jdaviz-3.8.2/jdaviz/components/plugin_file_import_select.vue` & `jdaviz-3.9.0/jdaviz/components/plugin_file_import_select.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/components/plugin_layer_select.vue` & `jdaviz-3.9.0/jdaviz/components/plugin_layer_select.vue`

 * *Files 4% similar despite different names*

```diff
@@ -16,20 +16,20 @@
       item-value="label"
       persistent-hint
     >
     <template slot="selection" slot-scope="data">
       <div class="single-line" style="width: 100%">
         <v-chip v-if="multiselect" style="width: calc(100% - 10px)">
           <span>
-            <j-layer-viewer-icon :icon="data.item.icon" :prevent_invert_if_dark="true"></j-layer-viewer-icon>
+            <j-layer-viewer-icon :icon="data.item.icon" :icons="icons" :prevent_invert_if_dark="true"></j-layer-viewer-icon>
             {{ data.item.label }}
           </span>
         </v-chip>
         <span v-else>
-          <j-layer-viewer-icon span_style="margin-right: 4px" :icon="data.item.icon" :prevent_invert_if_dark="true"></j-layer-viewer-icon>
+          <j-layer-viewer-icon span_style="margin-right: 4px" :icon="data.item.icon" :icons="icons" :prevent_invert_if_dark="true"></j-layer-viewer-icon>
           {{ data.item.label }}
         </span>
       </div>
     </template>
     <template v-slot:prepend-item v-if="multiselect">
       <v-list-item
         ripple
@@ -48,27 +48,27 @@
         </v-list-item-content>
       </v-list-item>
       <v-divider class="mt-2"></v-divider>
     </template>
     <template slot="item" slot-scope="data">
       <div class="single-line">
         <span>
-          <j-layer-viewer-icon span_style="margin-right: 4px" :icon="data.item.icon" :prevent_invert_if_dark="true"></j-layer-viewer-icon>
+          <j-layer-viewer-icon span_style="margin-right: 4px" :icon="data.item.icon" :icons="icons" :prevent_invert_if_dark="true"></j-layer-viewer-icon>
           {{ data.item.label }}
         </span>
       </div>
     </template>
    </v-select>
   </v-row>
  </div>
 </template>
 
 <script>
 module.exports = {
-  props: ['items', 'selected', 'label', 'hint', 'rules', 'show_if_single_entry', 'multiselect']
+  props: ['items', 'selected', 'label', 'hint', 'rules', 'icons', 'show_if_single_entry', 'multiselect']
 };
 </script>
 
 <style scoped>
   .v-select__selections {
     flex-wrap: nowrap !important;
     display: block !important;
```

### Comparing `jdaviz-3.8.2/jdaviz/components/plugin_layer_select_tabs.vue` & `jdaviz-3.9.0/jdaviz/components/plugin_layer_select_tabs.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/components/plugin_plot.vue` & `jdaviz-3.9.0/jdaviz/components/plugin_plot.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/components/plugin_section_header.vue` & `jdaviz-3.9.0/jdaviz/components/plugin_section_header.vue`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,57 @@
 00000000: 3c74 656d 706c 6174 653e 0a20 203c 6469  <template>.  <di
-00000010: 7620 636c 6173 733d 2273 7472 696b 6520  v class="strike 
-00000020: 7465 7874 2d2d 7365 636f 6e64 6172 7922  text--secondary"
-00000030: 3e0a 2020 2020 203c 7370 616e 3e0a 2020  >.     <span>.  
-00000040: 2020 2020 203c 736c 6f74 3e3c 2f73 6c6f       <slot></slo
-00000050: 743e 0a20 2020 2020 3c2f 7370 616e 3e0a  t>.     </span>.
-00000060: 2020 3c2f 6469 763e 0a3c 2f74 656d 706c    </div>.</templ
-00000070: 6174 653e 0a0a 0a3c 7374 796c 6520 7363  ate>...<style sc
-00000080: 6f70 6564 3e0a 2e73 7472 696b 6520 7b0a  oped>..strike {.
-00000090: 2020 2020 6469 7370 6c61 793a 2062 6c6f      display: blo
-000000a0: 636b 3b0a 2020 2020 7465 7874 2d61 6c69  ck;.    text-ali
-000000b0: 676e 3a20 6365 6e74 6572 3b0a 2020 2020  gn: center;.    
-000000c0: 6f76 6572 666c 6f77 3a20 6869 6464 656e  overflow: hidden
-000000d0: 3b0a 2020 2020 7768 6974 652d 7370 6163  ;.    white-spac
-000000e0: 653a 206e 6f77 7261 703b 200a 2020 2020  e: nowrap; .    
-000000f0: 6d61 7267 696e 2d6c 6566 743a 202d 3132  margin-left: -12
-00000100: 7078 3b0a 2020 2020 6d61 7267 696e 2d72  px;.    margin-r
-00000110: 6967 6874 3a20 2d31 3270 783b 0a20 2020  ight: -12px;.   
-00000120: 206d 6172 6769 6e2d 746f 703a 2033 3670   margin-top: 36p
-00000130: 783b 0a20 2020 206d 6172 6769 6e2d 626f  x;.    margin-bo
-00000140: 7474 6f6d 3a20 3870 783b 0a7d 0a0a 2e73  ttom: 8px;.}...s
-00000150: 7472 696b 6520 3e20 7370 616e 207b 0a20  trike > span {. 
-00000160: 2020 2070 6f73 6974 696f 6e3a 2072 656c     position: rel
-00000170: 6174 6976 653b 0a20 2020 2064 6973 706c  ative;.    displ
-00000180: 6179 3a20 696e 6c69 6e65 2d62 6c6f 636b  ay: inline-block
-00000190: 3b0a 7d0a 0a2e 7374 7269 6b65 203e 2073  ;.}...strike > s
-000001a0: 7061 6e3a 6265 666f 7265 2c0a 2e73 7472  pan:before,..str
-000001b0: 696b 6520 3e20 7370 616e 3a61 6674 6572  ike > span:after
-000001c0: 207b 0a20 2020 2063 6f6e 7465 6e74 3a20   {.    content: 
-000001d0: 2222 3b0a 2020 2020 706f 7369 7469 6f6e  "";.    position
-000001e0: 3a20 6162 736f 6c75 7465 3b0a 2020 2020  : absolute;.    
-000001f0: 746f 703a 2035 3025 3b0a 2020 2020 7769  top: 50%;.    wi
-00000200: 6474 683a 2039 3939 3970 783b 0a20 2020  dth: 9999px;.   
-00000210: 2068 6569 6768 743a 2031 7078 3b0a 2020   height: 1px;.  
-00000220: 2020 6261 636b 6772 6f75 6e64 3a20 7267    background: rg
-00000230: 6261 2830 2c20 302c 2030 2c20 302e 3135  ba(0, 0, 0, 0.15
-00000240: 293b 0a7d 0a0a 2e73 7472 696b 6520 3e20  );.}...strike > 
-00000250: 7370 616e 3a62 6566 6f72 6520 7b0a 2020  span:before {.  
-00000260: 2020 7269 6768 743a 2031 3030 253b 0a20    right: 100%;. 
-00000270: 2020 206d 6172 6769 6e2d 7269 6768 743a     margin-right:
-00000280: 2031 3570 783b 0a7d 0a0a 2e73 7472 696b   15px;.}...strik
-00000290: 6520 3e20 7370 616e 3a61 6674 6572 207b  e > span:after {
-000002a0: 0a20 2020 206c 6566 743a 2031 3030 253b  .    left: 100%;
-000002b0: 0a20 2020 206d 6172 6769 6e2d 6c65 6674  .    margin-left
-000002c0: 3a20 3135 7078 3b0a 7d0a 3c2f 7374 796c  : 15px;.}.</styl
-000002d0: 653e 0a                                  e>.
+00000010: 7620 3a63 6c61 7373 3d22 6163 7469 7665  v :class="active
+00000020: 203f 2027 7374 7269 6b65 2073 7472 696b   ? 'strike strik
+00000030: 652d 6163 7469 7665 273a 2027 7374 7269  e-active': 'stri
+00000040: 6b65 2722 3e0a 2020 2020 203c 7370 616e  ke'">.     <span
+00000050: 3e0a 2020 2020 2020 203c 736c 6f74 3e3c  >.       <slot><
+00000060: 2f73 6c6f 743e 0a20 2020 2020 3c2f 7370  /slot>.     </sp
+00000070: 616e 3e0a 2020 3c2f 6469 763e 0a3c 2f74  an>.  </div>.</t
+00000080: 656d 706c 6174 653e 0a0a 3c73 6372 6970  emplate>..<scrip
+00000090: 743e 0a6d 6f64 756c 652e 6578 706f 7274  t>.module.export
+000000a0: 7320 3d20 7b0a 2020 7072 6f70 733a 205b  s = {.  props: [
+000000b0: 2761 6374 6976 6527 5d2c 0a7d 3b0a 3c2f  'active'],.};.</
+000000c0: 7363 7269 7074 3e0a 0a0a 3c73 7479 6c65  script>...<style
+000000d0: 2073 636f 7065 643e 0a2e 7374 7269 6b65   scoped>..strike
+000000e0: 207b 0a20 2020 2064 6973 706c 6179 3a20   {.    display: 
+000000f0: 626c 6f63 6b3b 0a20 2020 2074 6578 742d  block;.    text-
+00000100: 616c 6967 6e3a 2063 656e 7465 723b 0a20  align: center;. 
+00000110: 2020 206f 7665 7266 6c6f 773a 2068 6964     overflow: hid
+00000120: 6465 6e3b 0a20 2020 2077 6869 7465 2d73  den;.    white-s
+00000130: 7061 6365 3a20 6e6f 7772 6170 3b20 0a20  pace: nowrap; . 
+00000140: 2020 206d 6172 6769 6e2d 6c65 6674 3a20     margin-left: 
+00000150: 2d31 3270 783b 0a20 2020 206d 6172 6769  -12px;.    margi
+00000160: 6e2d 7269 6768 743a 202d 3132 7078 3b0a  n-right: -12px;.
+00000170: 2020 2020 6d61 7267 696e 2d74 6f70 3a20      margin-top: 
+00000180: 3336 7078 3b0a 2020 2020 6d61 7267 696e  36px;.    margin
+00000190: 2d62 6f74 746f 6d3a 2038 7078 3b0a 7d0a  -bottom: 8px;.}.
+000001a0: 0a2e 7374 7269 6b65 203e 2073 7061 6e20  ..strike > span 
+000001b0: 7b0a 2020 2020 706f 7369 7469 6f6e 3a20  {.    position: 
+000001c0: 7265 6c61 7469 7665 3b0a 2020 2020 6469  relative;.    di
+000001d0: 7370 6c61 793a 2069 6e6c 696e 652d 626c  splay: inline-bl
+000001e0: 6f63 6b3b 0a7d 0a0a 2e73 7472 696b 6520  ock;.}...strike 
+000001f0: 3e20 7370 616e 3a62 6566 6f72 652c 0a2e  > span:before,..
+00000200: 7374 7269 6b65 203e 2073 7061 6e3a 6166  strike > span:af
+00000210: 7465 7220 7b0a 2020 2020 636f 6e74 656e  ter {.    conten
+00000220: 743a 2022 223b 0a20 2020 2070 6f73 6974  t: "";.    posit
+00000230: 696f 6e3a 2061 6273 6f6c 7574 653b 0a20  ion: absolute;. 
+00000240: 2020 2074 6f70 3a20 3530 253b 0a20 2020     top: 50%;.   
+00000250: 2077 6964 7468 3a20 3939 3939 7078 3b0a   width: 9999px;.
+00000260: 2020 2020 6865 6967 6874 3a20 3170 783b      height: 1px;
+00000270: 0a20 2020 2062 6163 6b67 726f 756e 643a  .    background:
+00000280: 2067 7261 793b 0a7d 0a0a 2e73 7472 696b   gray;.}...strik
+00000290: 652d 6163 7469 7665 203e 2073 7061 6e3a  e-active > span:
+000002a0: 6265 666f 7265 2c0a 2e73 7472 696b 652d  before,..strike-
+000002b0: 6163 7469 7665 203e 2073 7061 6e3a 6166  active > span:af
+000002c0: 7465 7220 7b0a 2020 2020 6261 636b 6772  ter {.    backgr
+000002d0: 6f75 6e64 3a20 2363 3735 6432 633b 2020  ound: #c75d2c;  
+000002e0: 2f2a 2061 6374 6976 6520 6f72 616e 6765  /* active orange
+000002f0: 202a 2f0a 7d0a 0a2e 7374 7269 6b65 203e   */.}...strike >
+00000300: 2073 7061 6e3a 6265 666f 7265 207b 0a20   span:before {. 
+00000310: 2020 2072 6967 6874 3a20 3130 3025 3b0a     right: 100%;.
+00000320: 2020 2020 6d61 7267 696e 2d72 6967 6874      margin-right
+00000330: 3a20 3135 7078 3b0a 7d0a 0a2e 7374 7269  : 15px;.}...stri
+00000340: 6b65 203e 2073 7061 6e3a 6166 7465 7220  ke > span:after 
+00000350: 7b0a 2020 2020 6c65 6674 3a20 3130 3025  {.    left: 100%
+00000360: 3b0a 2020 2020 6d61 7267 696e 2d6c 6566  ;.    margin-lef
+00000370: 743a 2031 3570 783b 0a7d 0a3c 2f73 7479  t: 15px;.}.</sty
+00000380: 6c65 3e0a                                le>.
```

### Comparing `jdaviz-3.8.2/jdaviz/components/plugin_subset_select.vue` & `jdaviz-3.9.0/jdaviz/components/plugin_subset_select.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/components/plugin_table.vue` & `jdaviz-3.9.0/jdaviz/components/plugin_table.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/components/plugin_viewer_select.vue` & `jdaviz-3.9.0/jdaviz/components/plugin_viewer_select.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/components/toolbar_nested.py` & `jdaviz-3.9.0/jdaviz/components/toolbar_nested.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,25 +49,25 @@
                 tool = tool_cls(viewer)
                 self.add_tool(tool,
                               menu_ind=menu_ind,
                               has_suboptions=len(subtools) > 1,
                               primary=i == 0,
                               visible=True)
 
-        # handle logic for tool visibilities (which will also handle setting the primary
-        # to something other than the first entry, if necessary)
-        self._update_tool_visibilities()
-
         # default_tool_priority allows falling back on an existing tool
         # if its the primary tool.  If no items in default_tool_priority
         # are currently "primary", then either no tool will be selected
         # or will fallback on BasicJupyterToolbar's handling of
         # viewer._default_mouse_mode_cls (which will not show that tool as active).
         self.default_tool_priority = default_tool_priority
-        self._handle_default_tool()
+
+        # handle logic for tool visibilities (which will also handle setting the primary
+        # to something other than the first entry, if necessary)
+        # NOTE: this will also call _handle_default_tool
+        self._update_tool_visibilities()
 
         # toolbars in the main app viewers need to respond to the data-collection, etc,
         # but those in plugins do not
         if hasattr(self.viewer, 'hub'):
             for msg in (AddDataMessage, RemoveDataMessage, ViewerAddedMessage, ViewerRemovedMessage,
                         SpectralMarksChangedMessage):
                 self.viewer.hub.subscribe(self, msg,
@@ -128,14 +128,15 @@
                 self.tools_data[tool_id] = {**self.tools_data[tool_id],
                                             'has_suboptions': n_visible > 1}
 
         # mutation to dictionary needs to be manually sent to update the UI
         self.send_state("tools_data")
         if needs_deactivate_active:
             self.active_tool_id = None
+        self._handle_default_tool()
 
     def _handle_default_tool(self):
         # default to the first item in the default_tool_priority list that is currently
         # already primary
         for tool_id in self.default_tool_priority:
             if tool_id not in self.tools_data:
                 continue
```

### Comparing `jdaviz-3.8.2/jdaviz/components/toolbar_nested.vue` & `jdaviz-3.9.0/jdaviz/components/toolbar_nested.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/components/tooltip.vue` & `jdaviz-3.9.0/jdaviz/components/tooltip.vue`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 // html.  If enabling a new tooltip, wrap the element in <j-tooltip tipid='...'>,
 // pass doctips from state/props, and test to make sure layout isn't adversely
 // affected by the wrapping divs.
 const tooltips = {
   // app toolbar
   'app-help': 'Open docs in new tab',
   'app-snackbar-history': 'Toggle logger overlay',
-  'app-toolbar-plugins': 'Data analysis plug-ins',
+  'app-toolbar-plugins': 'Toggle plugin sidebar',
   'app-toolbar-popout': `Display in a new window<br /><br />
     <div style="width: 200px; border: 1px solid gray;" class="pa-2">
       <strong>Note:</strong>
       some ad blockers or browser settings may block popup windows,
       causing this feature not to work.
     </div>`,
   'plugin-popout': `Display in a new window<br /><br />
@@ -36,14 +36,16 @@
       <strong>Note:</strong>
       some ad blockers or browser settings may block popup windows,
       causing this feature not to work.
     </div>`, 
 
   'g-data-tools': 
     'Load data from file',
+  'g-viewer-creator':
+     'Create a new viewer',
   'g-subset-tools': 
     'Select, create, and delete subsets',
   'g-subset-mode':
     'Operation performed by subset selection in viewer',
   'g-unified-slider':
     'Grab slider to slice through cube or select slice number',
   'g-redshift-slider':
@@ -62,15 +64,17 @@
   'viewer-toolbar-more': 'More options...',
   'viewer-data-select-enabled': 'Allow multiple entries (click to enable replace)',
   'viewer-data-radio-enabled': 'Replace current entry (click to enable multi-select)',
   'viewer-data-select': 'Toggle visibility of all layers associated with this data entry',
   'viewer-data-radio': 'Switch visibility to layers associated with this data entry',
   'viewer-data-enable': 'Load data entry into this viewer',
   'viewer-data-disable': 'Disable data within this viewer (will be hidden and unavailable from plugins until re-enabled)',
+  'viewer-wcs-delete': 'Remove orientation option across entire app',
   'viewer-data-delete': 'Remove data entry across entire app (might affect existing subsets)',
+  'viewer-data-nowcs': 'Data does not have WCS, cannot add unless link type changed to pixel',
 
   'table-prev': 'Select previous row in table',
   'table-next': 'Select next row in table',
   'table-play-pause-toggle': 'Toggle cycling through rows of table',
   'table-play-pause-delay': 'Set delay before cycling to next entry',
   'viewer-multiselect-toggle': 'Toggle between choosing a single or multiple viewer(s)',
   'layer-multiselect-toggle': 'Toggle between choosing a single or multiple layer(s)',
@@ -93,14 +97,16 @@
   'plugin-line-lists-line-visible': 'Toggle showing the line in the spectrum viewer',
   'plugin-line-lists-line-identify': 'Highlight this line in the spectrum viewer for easy identification',
   'plugin-line-lists-color-picker': 'Change the color of this list',
   'plugin-line-lists-spectral-range': 'Toggle filter to only lines observable within the range of the Spectrum Viewer',
   'plugin-line-analysis-sync-identify': 'Lock/unlock selection with identified line',
   'plugin-line-analysis-assign': 'Assign the centroid wavelength and update the redshift',
   'plugin-moment-save-fits': 'Save moment map as FITS file',
+  'plugin-extract-save-fits': 'Save spectral extraction as FITS file',
+  'plugin-collapse-save-fits': 'Save collapsed cube as FITS file',
   'plugin-link-apply': 'Apply linking to data',
   'plugin-footprints-color-picker': 'Change the color of the footprint overlay',
 }
 
 
 module.exports = {
   props: ['tooltipcontent', 'tipid', 'delay', 'nudgebottom', 'span_style'],
```

### Comparing `jdaviz-3.8.2/jdaviz/components/tray_plugin.vue` & `jdaviz-3.9.0/jdaviz/components/tray_plugin.vue`

 * *Files 10% similar despite different names*

```diff
@@ -13,42 +13,46 @@
       <span> {{ getDisabledMsg() }}</span>
     </v-row>
     <div v-else>
       <v-row v-if="uses_active_status && keep_active !== undefined" style="padding-bottom: 24px">
         <v-switch
           v-model="keep_active"
           @change="$emit('update:keep_active', $event)"
-          label="keep active"
-          hint="consider plugin active (showing any previews and enabling all keypress events) even when not opened"
+          label="Keep active"
+          hint="Consider plugin active (showing any previews and enabling all keypress events) even when not opened"
           persistent-hint>
         </v-switch>
       </v-row>
       <slot></slot>
     </div>
   </v-container>
 </template>
 
 <script>
 module.exports = {
-  props: ['disabled_msg', 'description', 'link', 'popout_button',
-          'uses_active_status', 'keep_active'],
+  props: ['irrelevant_msg', 'disabled_msg', 'description', 'link', 'popout_button',
+          'uses_active_status', 'keep_active', 'scroll_to'],
   methods: {
     isDisabled() {
       return this.getDisabledMsg().length > 0
     },
     getDisabledMsg() {
-      return this.disabled_msg || ''
+      return this.irrelevant_msg || this.disabled_msg || ''
     },
     sendPing(recursive) {
       if (!this.$el.isConnected) {
         return
       }
       if (!document.hidden) {
         this.$emit('plugin-ping', Date.now())
       }
+      if (this.scroll_to) {
+        this.$emit('update:scroll_to', false)
+        this.$el.scrollIntoView({behavior: "smooth", block: "nearest", inline: "start"});
+      }
       if (!recursive) {
         return
       }
       setTimeout(() => {
         this.sendPing(true)          
       }, 200)  // ms
     }
```

### Comparing `jdaviz-3.8.2/jdaviz/components/viewer_data_select.vue` & `jdaviz-3.9.0/jdaviz/components/viewer_data_select.vue`

 * *Files 10% similar despite different names*

```diff
@@ -44,55 +44,73 @@
           </span>
         </v-row>
 
         <v-row v-for="item in filteredDataItems" :key="item.id" style="padding-left: 25px; margin-right: 0px; margin-top: 4px; margin-bottom: 4px">
           <j-viewer-data-select-item
             :item="item"
             :icon="layer_icons[item.name]"
+            :icons="icons"
             :viewer="viewer"
             :multi_select="multi_select"
+            :is_wcs_only="false"
             :n_data_entries="nDataEntries"
             @data-item-visibility="$emit('data-item-visibility', $event)"
             @data-item-unload="$emit('data-item-unload', $event)"
             @data-item-remove="$emit('data-item-remove', $event)"
           ></j-viewer-data-select-item>
         </v-row>
 
-        <div v-if="extraDataItems.length" style="margin-bottom: -8px;">
+        <div v-if="linkedByWcs()">
+          <j-plugin-section-header style="margin-top: 0px">Orientation</j-plugin-section-header>
+          <v-row v-for="item in wcsOnlyItems" :key="item.id" style="padding-left: 25px; margin-right: -8px; margin-top: 4px; margin-bottom: 4px">
+            <j-viewer-data-select-item
+              :item="item"
+              :icon="layer_icons[item.name]"
+              :icons="icons"
+              :viewer="viewer"
+              :multi_select="multi_select"
+              :is_wcs_only="true"
+              @data-item-remove="$emit('data-item-remove', $event)"
+              @change-reference-data="$emit('change-reference-data', $event)"
+            ></j-viewer-data-select-item>
+          </v-row>
+        </div>
+
+        <div v-if="extraDataItems.length > 0" style="margin-bottom: -8px;">
           <v-row key="extra-items-expand" style="padding-left: 25px; margin-right: 0px; padding-bottom: 4px; background-color: #E3F2FD"> 
             <span 
               @click="toggleShowExtraItems"
-              class='text--primary' 
+              class='text--primary'
               style="overflow-wrap: anywhere; font-size: 12pt; padding-top: 6px; padding-left: 6px; cursor: pointer"
             >
               <v-icon class='invert-if-dark'>{{showExtraItems ? 'mdi-chevron-double-up' : 'mdi-chevron-double-down'}}</v-icon>
               <span v-if="viewer.config === 'mosviz'">
                 {{showExtraItems ? 'hide other row data not in viewer' : 'show other row data not in viewer'}}
               </span>
               <span v-else>
-                {{showExtraItems ? 'hide data not in viewer' : 'show data not in viewer'}}                
+                {{showExtraItems ? 'hide data not in viewer' : 'show data not in viewer'}}
               </span>
             </span>
           </v-row>
 
-          <v-row v-if="showExtraItems" v-for="item in extraDataItems"  :key="item.id" style="padding-left: 25px; margin-right: 0px; margin-top: 4px; margin-bottom: 4px">
+          <v-row v-if="showExtraItems" v-for="item in extraDataItems" :key="item.id" style="padding-left: 25px; margin-right: 0px; margin-top: 4px; margin-bottom: 4px">
             <j-viewer-data-select-item
               :item="item"
               :icon="layer_icons[item.name]"
+              :icons="icons"
               :viewer="viewer"
               :multi_select="multi_select"
+              :is_wcs_only="false"
               :n_data_entries="nDataEntries"
               @data-item-visibility="$emit('data-item-visibility', $event)"
               @data-item-remove="$emit('data-item-remove', $event)"
             ></j-viewer-data-select-item>
           </v-row>
         </div>
-
       </v-list>
-
     </v-menu>
     <div :id="'target-' + viewer.id"></div>
   </j-tooltip>
 </template>
 <script>
 
 module.exports = {
@@ -107,23 +125,27 @@
       if (['image-viewer', 'spectrum-2d-viewer'].indexOf(this.$props.viewer.reference) !== -1) {
         multi_select = false
       }
     } else if (this.$props.viewer.config === 'specviz2d') {
       if (this.$props.viewer.reference === 'spectrum-2d-viewer') {
         multi_select = false
       }
+    } else if (this.$props.viewer.config === 'lcviz') {
+      if (this.$props.viewer.reference.startsWith('image')) {
+        multi_select = false
+      }
     }
     return {
       // default to passed values, whenever value or uncertainty are changed
       // updateTruncatedValues will overwrite the displayed values
-      data_menu_open: false,
+      data_menu_open: this.$props.viewer.open_data_menu_if_empty && Object.keys(this.$props.viewer.selected_data_items).length == 0 && this.$props.data_items.length > 0,
       multi_select: multi_select,
       showExtraItems: Object.keys(this.$props.viewer.selected_data_items).length == 0,
       valueTrunc: this.value,
-      uncertTrunc: this.uncertainty
+      uncertTrunc: this.uncertainty,
     }
   },
   mounted() {
     let element = document.getElementById(`target-${this.viewer.id}`).parentElement
     if (element === null) {
       return
     }
@@ -159,20 +181,22 @@
       if (this.$props.viewer.reference === 'table-viewer') {
         return false
       }
       return true
     },
     dataItemInViewer(item, returnExtraItems) {
       const inViewer = Object.keys(this.$props.viewer.selected_data_items).includes(item.id)
-      //console.log(item.name+"  "+inViewer)
       if (returnExtraItems) {
         return (!inViewer && (item.meta.mosviz_row === this.$props.app_settings.mosviz_row))
       }
       return inViewer
     },
+    wcsOnlyItem(item) {
+      return item.type == 'wcs-only'
+    },
     itemIsVisible(item, returnExtraItems) {
       if (this.$props.viewer.config === 'mosviz') {
         if (this.$props.viewer.reference === 'spectrum-viewer' && item.type !== '1d spectrum') {
           // filters out table, spectrum 2d, images
           return false
         } else if (this.$props.viewer.reference === 'spectrum-2d-viewer' && item.type !== '2d spectrum') {
           return false
@@ -203,48 +227,65 @@
         if (this.$props.viewer.reference === 'spectrum-viewer') {
           return item.ndims === 1 && item.type!=='trace' && this.dataItemInViewer(item, returnExtraItems)
         } else if (this.$props.viewer.reference === 'spectrum-2d-viewer') {
           return (item.ndims === 2 || item.type==='trace') && this.dataItemInViewer(item, returnExtraItems)
         }
       } else if (this.$props.viewer.config === 'lcviz') {
         // TODO: generalize itemIsVisible so downstream apps can provide their own customized filters
+        if (this.$props.viewer.reference.startsWith('image')) {
+          return (item.ndims === 3 && this.dataItemInViewer(item, returnExtraItems))
+        }
         if (item.meta._LCVIZ_EPHEMERIS !== undefined) {
           if (!this.$props.viewer.reference.startsWith('flux-vs-phase:')) {
             return false
           }
-          var viewer_ephem_comp = this.$props.viewer.reference.split('flux-vs-phase:')[1]
-          return item.meta._LCVIZ_EPHEMERIS.ephemeris == viewer_ephem_comp && this.dataItemInViewer(item, returnExtraItems)
+          var viewer_ephem_comp = this.$props.viewer.reference.split('flux-vs-phase:')[1].split('[')[0]
+          return item.ndims === 1 && item.meta._LCVIZ_EPHEMERIS.ephemeris == viewer_ephem_comp && this.dataItemInViewer(item, returnExtraItems)
         }
-        return this.dataItemInViewer(item, returnExtraItems)
+        return item.ndims === 1 && this.dataItemInViewer(item, returnExtraItems)
+      } else if (this.$props.viewer.config === 'imviz') {
+        return this.dataItemInViewer(item, returnExtraItems && !this.wcsOnlyItem(item))
       }
       // for any situation not covered above, default to showing the entry
       return this.dataItemInViewer(item, returnExtraItems)
     },
     toggleShowExtraItems() {
       // toggle the visibility of the extra items in the menu
       this.showExtraItems = !this.showExtraItems
     },
     toggleMultiSelect() {
       this.multi_select = !this.multi_select
-      if (this.multi_select === false){
+      if (this.multi_select === false) {
         // If we're toggling to single select, set the first item visibility to replace the rest
         // Find the "first" item
-        for (item_index in this.filteredDataItems){
+        for (item_index in this.filteredDataItems) {
           if (this.$props.viewer.selected_data_items[this.filteredDataItems[item_index].id] === 'visible') {
             this.$emit('data-item-visibility', {
               id: this.$props.viewer.id,
               item_id: this.filteredDataItems[item_index].id,
               visible: true,
-              replace: true})
+              replace: true
+            })
             break;
           }
         }
       }
-      
     },
+    isRefData() {
+      return this.$props.item.viewer.reference_data_label === this.$props.item.name
+    },
+    selectRefData() {
+      this.$emit('change-reference-data', {
+        id: this.$props.viewer.id,
+        item_id: this.$props.item.id
+      })
+    },
+    linkedByWcs() {
+      return this.$props.viewer.linked_by_wcs
+    }
   },
   computed: {
     viewerTitleCase() {
       var title = this.$props.viewer.reference || this.$props.viewer.id
       // this translates from kebab-case to human readable (individual words, in title case)
       // each word that should NOT be capitalized needs to explicitly be set here
       return title.toLowerCase().replaceAll('-', ' ').split(' ').map((word) => {if (['vs'].indexOf(word) !== -1) {return word} else {return word.charAt(0).toUpperCase() + word.slice(1)}}).join(' ');
@@ -263,10 +304,13 @@
     extraDataItems() {
       return this.$props.data_items.filter((item) => this.itemIsVisible(item, true))
     },
     nDataEntries() {
       // return number of data entries in the entire plugin that were NOT created by a plugin
       return this.$props.data_items.filter((item) => item.meta.Plugin === undefined).length
     },
+    wcsOnlyItems() {
+      return this.$props.data_items.filter((item) => this.wcsOnlyItem(item))
+    },
   }
 };
 </script>
```

### Comparing `jdaviz-3.8.2/jdaviz/components/viewer_data_select_item.vue` & `jdaviz-3.9.0/jdaviz/components/viewer_data_select_item.vue`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,58 @@
 <template>
   <div style="display: contents">
-    <div v-if="isSelected">
+    <div v-if="is_wcs_only">
+      <j-tooltip
+        :tooltipcontent="isRefData() ? 'Current viewer orientation' : 'Set as viewer orientation'"
+        span_style="width: 36px"
+      >
+        <v-btn 
+          icon
+          :color="isRefData() ? 'accent' : 'default'"
+          @click="selectRefData">
+            <v-icon>{{isRefData() ? "mdi-radiobox-marked" : "mdi-radiobox-blank"}}</v-icon>
+        </v-btn>
+      </j-tooltip>
+    </div>
+    <div v-else-if="isSelected">
       <j-tooltip :tipid="multi_select ? 'viewer-data-select' : 'viewer-data-radio'">
         <v-btn 
           icon
           :color="visibleState==='visible' ? 'accent' : 'default'"
           @click="selectClicked">
             <v-icon v-if="multi_select || item.type==='trace'">{{visibleState!=='hidden' ? "mdi-checkbox-marked" : "mdi-checkbox-blank-outline"}}</v-icon>
             <v-icon v-else>{{visibleState!=='hidden' ? "mdi-radiobox-marked" : "mdi-radiobox-blank"}}</v-icon>
         </v-btn>
       </j-tooltip>
     </div>
-    <div v-else>
+    <div v-else-if="!linkedByWcs() || item.has_wcs || item.is_astrowidgets_markers_table">
       <j-tooltip tipid="viewer-data-enable">
-        <v-btn 
+        <v-btn
           icon
           color="default"
           @click="selectClicked">
             <v-icon>mdi-plus</v-icon>
         </v-btn>
       </j-tooltip>
     </div>
+    <div v-else>
+      <j-tooltip tipid="viewer-data-nowcs">
+        <v-btn
+          icon
+          color="default"
+          disabled>
+          <v-icon>mdi-plus</v-icon>
+        </v-btn>
+      </j-tooltip>
+    </div>
+
+    <j-tooltip :tooltipcontent="is_wcs_only ? '' : 'data label: '+item.name" span_style="font-size: 12pt; padding-top: 6px; padding-left: 4px; padding-right: 16px; width: calc(100% - 80px); white-space: nowrap; cursor: default;">
+      <j-layer-viewer-icon span_style="margin-left: 4px;" :icon="icon" :icons="icons" color="#000000DE"></j-layer-viewer-icon>
 
-    <j-tooltip :tooltipcontent="'data label: '+item.name" span_style="font-size: 12pt; padding-top: 6px; padding-left: 4px; padding-right: 16px; width: calc(100% - 80px); white-space: nowrap; cursor: default;">
-      <j-layer-viewer-icon span_style="margin-left: 4px; margin-right: 4px" :icon="icon" color="#000000DE"></j-layer-viewer-icon>
-      <div class="text-ellipsis-middle" style="font-weight: 500">
+      <div class="text-ellipsis-middle" style="font-weight: 500;">
         <span>
           {{itemNamePrefix}}
         </span>
         <span>
           {{itemNameExtension}}
         </span>
       </div>
@@ -43,57 +67,70 @@
             item_id: item.id
           })"
         ><v-icon>mdi-close</v-icon></v-btn>
       </j-tooltip>
     </div>
 
     <div v-if="isDeletable" style="padding-left: 2px; right: 2px">
-      <j-tooltip tipid='viewer-data-delete'>
+      <j-tooltip :tipid="is_wcs_only ? 'viewer-wcs-delete' : 'viewer-data-delete'">
         <v-btn
           icon
           @click="$emit('data-item-remove', {item_name: item.name, viewer_id: viewer.id})"
         ><v-icon>mdi-delete</v-icon></v-btn>
       </j-tooltip>
     </div>
   </div>
 </template>
 
 <script>
 
 module.exports = {
-  props: ['item', 'icon', 'multi_select', 'viewer', 'n_data_entries'],
+  props: ['item', 'icon', 'icons', 'multi_select', 'viewer', 'n_data_entries', 'is_wcs_only'],
   methods: {
     selectClicked() {
       prevVisibleState = this.visibleState
       // checkboxes control VISIBILITY of layers not loaded state
       // if we just loaded the data, its probably already visible, but we'll still make sure all
       // appropriate layers are visible and properly handle replace for non-multiselect
       // NOTE: replace=True will exclude removing trace items
       this.$emit('data-item-visibility', {
         id: this.$props.viewer.id,
         item_id: this.$props.item.id,
         visible: prevVisibleState != 'visible' || (!this.multi_select && this.$props.item.type !== 'trace'),
         replace: !this.multi_select && this.$props.item.type !== 'trace'
       })
-
+    },
+    selectRefData() {
+      if (this.linkedByWcs() && !this.isRefData() && this.is_wcs_only) {
+        this.$emit('change-reference-data', {
+          id: this.$props.viewer.id,
+          item_id: this.$props.item.id
+        })
+      }
+    },
+    isRefData() {
+      return this.$props.viewer.reference_data_label == this.$props.item.name
+    },
+    linkedByWcs() {
+      return this.$props.viewer.linked_by_wcs
     }
   },
   computed: {
     itemNamePrefix() {
       if (this.$props.item.name.indexOf("[") !== -1) {
         // return everything BEFORE the LAST [
         return this.$props.item.name.split('[').slice(0, -1).join()
       } else {
         return this.$props.item.name
       }
     },
     itemNameExtension() {
       if (this.$props.item.name.indexOf("[") !== -1) {
         // return the LAST [ and everything FOLLOWING
-        return '['+this.$props.item.name.split('[').slice(-1)
+        return '[' + this.$props.item.name.split('[').slice(-1)
       } else {
         return ''
       }
     },
     isSelected() {
       return Object.keys(this.$props.viewer.selected_data_items).includes(this.$props.item.id)
     },
@@ -135,15 +172,15 @@
     },
     isDeletable() {
       isLastDataset = (this.$props.n_data_entries <= 1)
       notSelected = !this.isSelected
       isMosviz = this.$props.viewer.config === 'mosviz'
       isCubeviz = this.$props.viewer.config === 'cubeviz'
       isPluginData = !(this.$props.item.meta.Plugin === undefined)
-      return notSelected && (isPluginData || (!isLastDataset && !isMosviz && !isCubeviz))
+      return notSelected && (isPluginData || (!isLastDataset && !isMosviz && !isCubeviz)) && (this.$props.item.name !== 'Default orientation')
     },
     selectTipId() {
       if (this.multi_select) {
         return 'viewer-data-select'
       } else {
         return 'viewer-data-radio'
       }
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/cubeviz/cubeviz.ipynb` & `jdaviz-3.9.0/jdaviz/configs/cubeviz/cubeviz.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/cubeviz/cubeviz.yaml` & `jdaviz-3.9.0/jdaviz/configs/specviz2d/specviz2d.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,40 @@
 settings:
-  configuration: cubeviz
-  data:
-    auto_populate: true
-    parser: cubeviz-data-parser
+  configuration: specviz2d
   visible:
     menu_bar: false
     toolbar: true
     tray: true
-    tab_headers: true
+    tab_headers: false
   dense_toolbar: false
   server_is_remote: false
   context:
     notebook:
-      max_height: 750px
+      max_height: 600px
 toolbar:
   - g-data-tools
   - g-subset-tools
   - g-coords-info
 tray:
   - g-metadata-viewer
   - g-plot-options
   - g-subset-plugin
   - g-markers
-  - cubeviz-slice
+  - spectral-extraction
   - g-gaussian-smooth
-  - g-collapse
   - g-model-fitting
   - g-line-list
   - specviz-line-analysis
-  - cubeviz-moment-maps
-  - cubeviz-spectral-extraction
-  - g-export-plot
+  - export
 viewer_area:
   - container: col
     children:
       - container: row
         viewers:
-          - name: Flux
-            plot: cubeviz-image-viewer
-            reference: flux-viewer
-          - name: Uncertainty
-            plot: cubeviz-image-viewer
-            reference: uncert-viewer
+          - name: 2D Spectrum viewer
+            plot: mosviz-profile-2d-viewer
+            reference: spectrum-2d-viewer
       - container: row
         viewers:
           - name: Spectrum
-            plot: cubeviz-profile-viewer
+            plot: mosviz-profile-viewer
             reference: spectrum-viewer
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/cubeviz/helper.py` & `jdaviz-3.9.0/jdaviz/configs/cubeviz/helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import numpy as np
 from astropy.io import fits
 from astropy.io import registry as io_registry
+from astropy.utils.decorators import deprecated
 from glue.core import BaseData
 from specutils import Spectrum1D
 from specutils.io.registers import _astropy_has_priorities
 
 from jdaviz.core.helpers import ImageConfigHelper
 from jdaviz.configs.default.plugins.line_lists.line_list_mixin import LineListMixin
 from jdaviz.configs.specviz import Specviz
 from jdaviz.core.events import (AddDataMessage,
                                 SliceSelectSliceMessage)
 
 __all__ = ['Cubeviz']
 
 
+_spectral_axis_names = ["Wave", "Wavelength", "Freq", "Frequency",
+                        "Wavenumber", "Velocity", "Energy"]
+
+
 class Cubeviz(ImageConfigHelper, LineListMixin):
     """Cubeviz Helper class"""
     _default_configuration = 'cubeviz'
     _default_spectrum_viewer_reference_name = "spectrum-viewer"
     _default_uncert_viewer_reference_name = "uncert-viewer"
     _default_flux_viewer_reference_name = "flux-viewer"
     _default_image_viewer_reference_name = "image-viewer"
@@ -32,16 +37,15 @@
 
     def _set_spectrum_x_axis(self, msg):
         viewer = self.app.get_viewer(self._default_spectrum_viewer_reference_name)
         if msg.viewer_id != viewer.reference_id:
             return
         ref_data = viewer.state.reference_data
         if ref_data and ref_data.ndim == 3:
-            for att_name in ["Wave", "Wavelength", "Freq", "Frequency",
-                             "Wavenumber", "Velocity", "Energy"]:
+            for att_name in _spectral_axis_names:
                 if att_name in ref_data.component_ids():
                     if viewer.state.x_att != ref_data.id[att_name]:
                         viewer.state.x_att = ref_data.id[att_name]
                         viewer.state.reset_limits()
                     break
             else:
                 viewer.state.x_att = ref_data.id["Pixel Axis 2 [x]"]
@@ -72,50 +76,44 @@
         if not override_cube_limit and len(self.app.state.data_items) != 0:
             raise RuntimeError('Only one cube may be loaded per Cubeviz instance')
         if data_label:
             kwargs['data_label'] = data_label
 
         super().load_data(data, parser_reference="cubeviz-data-parser", **kwargs)
 
+    @deprecated(since="3.9", alternative="select_wavelength")
     def select_slice(self, slice):
         """
         Select a slice by index.
 
         Parameters
         ----------
         slice : int
             Slice integer to select
         """
         if not isinstance(slice, int):
             raise TypeError("slice must be an integer")
         if slice < 0:
             raise ValueError("slice must be positive")
-        msg = SliceSelectSliceMessage(slice=slice, sender=self)
-        self.app.hub.broadcast(msg)
+        self.plugins['Slice'].slice = slice
 
     def select_wavelength(self, wavelength):
         """
         Select the slice closest to the provided wavelength.
 
         Parameters
         ----------
         wavelength : float
             Wavelength to select in units of the x-axis of the spectrum.  The nearest slice will
-            be selected.
+            be selected if "snap to slice" is enabled in the slice plugin.
         """
         if not isinstance(wavelength, (int, float)):
             raise TypeError("wavelength must be a float or int")
-        # Retrieve the x slices from the spectrum viewer's marks
-        sv = self.app.get_viewer(self._default_spectrum_viewer_reference_name)
-        x_all = sv.native_marks[0].x
-        if sv.state.layers[0].as_steps:
-            # then the marks have been doubled in length (each point duplicated)
-            x_all = x_all[::2]
-        index = np.argmin(abs(x_all - wavelength))
-        return self.select_slice(int(index))
+        msg = SliceSelectSliceMessage(value=wavelength, sender=self)
+        self.app.hub.broadcast(msg)
 
     @property
     def specviz(self):
         """
         A Specviz helper (:class:`~jdaviz.configs.specviz.helper.Specviz`) for the Jdaviz
         application that is wrapped by Cubeviz.
         """
@@ -164,14 +162,28 @@
                              " is set")
         elif function is False:
             function = None
         return self._get_data(data_label=data_label, spatial_subset=spatial_subset,
                               spectral_subset=spectral_subset, function=function,
                               cls=cls, use_display_units=use_display_units)
 
+    # Need this method for Imviz Aperture Photometry plugin.
+
+    def get_aperture_photometry_results(self):
+        """Return aperture photometry results, if any.
+        Results are calculated using :ref:`cubeviz-aper-phot` plugin.
+
+        Returns
+        -------
+        results : `~astropy.table.QTable` or `None`
+            Photometry results if available or `None` otherwise.
+
+        """
+        return self.plugins['Aperture Photometry']._obj.export_table()
+
 
 def layer_is_cube_image_data(layer):
     return isinstance(layer, BaseData) and layer.ndim in (2, 3)
 
 
 # TODO: We can remove this when specutils supports it, i.e.,
 #       https://github.com/astropy/specutils/issues/592 and
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.py` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/collapse/collapse.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,168 +1,167 @@
 import os
 from pathlib import Path
+import warnings
 
-from astropy import units as u
 from astropy.nddata import CCDData
+from glue.core import Data
+from specutils.manipulation import spectral_slab
+from traitlets import Bool, List, Unicode, observe
 
-from traitlets import Unicode, Bool, observe
-from specutils import manipulation, analysis
-
-from jdaviz.core.custom_traitlets import IntHandleEmpty
 from jdaviz.core.events import SnackbarMessage
 from jdaviz.core.registries import tray_registry
 from jdaviz.core.template_mixin import (PluginTemplateMixin,
                                         DatasetSelectMixin,
+                                        SelectPluginComponent,
                                         SpectralSubsetSelectMixin,
                                         AddResultsMixin,
                                         with_spinner)
 from jdaviz.core.user_api import PluginUserApi
 
-__all__ = ['MomentMap']
-
+__all__ = ['Collapse']
 
-spaxel = u.def_unit('spaxel', 1 * u.Unit(""))
-u.add_enabled_units([spaxel])
 
-
-@tray_registry('cubeviz-moment-maps', label="Moment Maps",
-               viewer_requirements=['spectrum', 'image'])
-class MomentMap(PluginTemplateMixin, DatasetSelectMixin, SpectralSubsetSelectMixin,
-                AddResultsMixin):
+@tray_registry('g-collapse', label="Collapse", viewer_requirements='spectrum')
+class Collapse(PluginTemplateMixin, DatasetSelectMixin, SpectralSubsetSelectMixin, AddResultsMixin):
     """
-    See the :ref:`Moment Maps Plugin Documentation <moment-maps>` for more details.
+    See the :ref:`Collapse Plugin Documentation <collapse>` for more details.
 
     Only the following attributes and methods are available through the
     :ref:`public plugin API <plugin-apis>`:
 
     * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.show`
     * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.open_in_tray`
     * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.close_in_tray`
     * ``dataset`` (:class:`~jdaviz.core.template_mixin.DatasetSelect`):
       Dataset to use for computing line statistics.
     * ``spectral_subset`` (:class:`~jdaviz.core.template_mixin.SubsetSelect`):
       Subset to use for the line, or ``Entire Spectrum``.
-    * ``n_moment``
     * ``add_results`` (:class:`~jdaviz.core.template_mixin.AddResults`)
-    * :meth:`calculate_moment`
+    * :meth:`collapse`
     """
-    template_file = __file__, "moment_maps.vue"
-
-    n_moment = IntHandleEmpty(0).tag(sync=True)
+    template_file = __file__, "collapse.vue"
+    function_items = List().tag(sync=True)
+    function_selected = Unicode('Sum').tag(sync=True)
     filename = Unicode().tag(sync=True)
-    moment_available = Bool(False).tag(sync=True)
+    collapsed_spec_available = Bool(False).tag(sync=True)
     overwrite_warn = Bool(False).tag(sync=True)
-
-    # export_enabled controls whether saving the moment map to a file is enabled via the UI.  This
+    # export_enabled controls whether saving to a file is enabled via the UI.  This
     # is a temporary measure to allow server-installations to disable saving server-side until
     # saving client-side is supported
     export_enabled = Bool(True).tag(sync=True)
 
     def __init__(self, *args, **kwargs):
+
         super().__init__(*args, **kwargs)
 
-        self.moment = None
+        self._label_counter = 0
+
+        self.collapsed_spec = None
+
+        self.function = SelectPluginComponent(self,
+                                              items='function_items',
+                                              selected='function_selected',
+                                              manual_options=['Mean', 'Median', 'Min', 'Max', 'Sum'])  # noqa
 
         self.dataset.add_filter('is_cube')
         self.add_results.viewer.filters = ['is_image_viewer']
 
         if self.app.state.settings.get('server_is_remote', False):
             # when the server is remote, saving the file in python would save on the server, not
             # on the user's machine, so export support in cubeviz should be disabled
             self.export_enabled = False
 
     @property
-    def _default_image_viewer_reference_name(self):
-        return self.jdaviz_helper._default_image_viewer_reference_name
-
-    @property
     def _default_spectrum_viewer_reference_name(self):
         return self.jdaviz_helper._default_spectrum_viewer_reference_name
 
     @property
     def user_api(self):
-        # NOTE: leaving save_as_fits out for now - we may want a more general API to do that
-        # accross all plugins at some point
-        return PluginUserApi(self, expose=('dataset', 'spectral_subset', 'n_moment',
-                                           'add_results', 'calculate_moment'))
+        return PluginUserApi(self, expose=('dataset', 'function', 'spectral_subset',
+                                           'add_results', 'collapse'))
 
-    @observe("dataset_selected", "dataset_items", "n_moment")
+    @observe("dataset_selected", "dataset_items")
     def _set_default_results_label(self, event={}):
         label_comps = []
         if hasattr(self, 'dataset') and len(self.dataset.labels) > 1:
             label_comps += [self.dataset_selected]
-        label_comps += [f"moment {self.n_moment}"]
+        label_comps += ["collapsed"]
         self.results_label_default = " ".join(label_comps)
 
     @with_spinner()
-    def calculate_moment(self, add_data=True):
+    def collapse(self, add_data=True):
         """
-        Calculate the moment map
+        Collapse over the spectral axis.
 
         Parameters
         ----------
         add_data : bool
-            Whether to add the resulting data object to the app according to ``add_results``.
+            Whether to load the resulting data back into the application according to
+            ``add_results``.
         """
-        # Retrieve the data cube and slice out desired region, if specified
-        if "_orig_spec" in self.dataset.selected_obj.meta:
-            cube = self.dataset.selected_obj.meta["_orig_spec"]
-        else:
-            cube = self.dataset.selected_obj
-
+        # Collapsing over the spectral axis. Cut out the desired spectral
+        # region. Defaults to the entire spectrum.
+        cube = self.dataset.selected_obj
         spec_min, spec_max = self.spectral_subset.selected_min_max(cube)
-        slab = manipulation.spectral_slab(cube, spec_min, spec_max)
 
-        # Calculate the moment and convert to CCDData to add to the viewers
-        try:
-            n_moment = int(self.n_moment)
-            if n_moment < 0:
-                raise ValueError("Moment must be a positive integer")
-        except ValueError:
-            raise ValueError("Moment must be a positive integer")
-        # Need transpose to align JWST mirror shape: This is because specutils
-        # arrange the array shape to be (nx, ny, nz) but 2D visualization
-        # assumes (ny, nx) as per row-major convention.
-        data_wcs = getattr(cube.wcs, 'celestial', None)
+        # Extract 2D WCS from input cube.
+        data = self.dataset.selected_dc_item
+        # Similar to coords_info logic.
+        if '_orig_spec' in getattr(data, 'meta', {}):
+            w = data.meta['_orig_spec'].wcs
+        else:
+            w = data.coords
+        data_wcs = getattr(w, 'celestial', None)
         if data_wcs:
             data_wcs = data_wcs.swapaxes(0, 1)  # We also transpose WCS to match.
-        self.moment = CCDData(analysis.moment(slab, order=n_moment).T, wcs=data_wcs)
 
-        fname_label = self.dataset_selected.replace("[", "_").replace("]", "")
-        self.filename = f"moment{n_moment}_{fname_label}.fits"
+        with warnings.catch_warnings():
+            warnings.filterwarnings('ignore', message='No observer defined on WCS')
+            spec = spectral_slab(cube, spec_min, spec_max)
+            # Spatial-spatial image only.
+            collapsed_spec = spec.collapse(self.function_selected.lower(), axis=-1).T  # Quantity
+
+            # stuff for exporting to file
+            self.collapsed_spec = CCDData(collapsed_spec, wcs=data_wcs)
+            self.collapsed_spec_available = True
+            fname_label = self.dataset_selected.replace("[", "_").replace("]", "")
+            self.filename = f"collapsed_{self.function_selected.lower()}_{fname_label}.fits"
 
         if add_data:
-            self.add_results.add_results_from_plugin(self.moment)
-
-            msg = SnackbarMessage("{} added to data collection".format(self.results_label),
-                                  sender=self, color="success")
-            self.hub.broadcast(msg)
+            data = Data(coords=data_wcs)
+            data['flux'] = collapsed_spec.value
+            data.get_component('flux').units = collapsed_spec.unit.to_string()
+
+            self.add_results.add_results_from_plugin(data)
+
+            snackbar_message = SnackbarMessage(
+                f"Data set '{self.dataset_selected}' collapsed successfully.",
+                color="success",
+                sender=self)
+            self.hub.broadcast(snackbar_message)
 
-        self.moment_available = True
+        return collapsed_spec
 
-        return self.moment
-
-    def vue_calculate_moment(self, *args):
-        self.calculate_moment(add_data=True)
+    def vue_collapse(self, *args, **kwargs):
+        self.collapse(add_data=True)
 
     def vue_save_as_fits(self, *args):
-        self._write_moment_to_fits()
+        self._save_collapsed_spec_to_fits()
 
     def vue_overwrite_fits(self, *args):
-        """Attempt to force writing the moment map if the user confirms the desire to overwrite."""
+        """Attempt to force writing the file if the user confirms the desire to overwrite."""
         self.overwrite_warn = False
-        self._write_moment_to_fits(overwrite=True)
+        self._save_collapsed_spec_to_fits(overwrite=True)
+
+    def _save_collapsed_spec_to_fits(self, overwrite=False, *args):
 
-    def _write_moment_to_fits(self, overwrite=False, *args):
-        if self.moment is None or not self.filename:  # pragma: no cover
-            return
         if not self.export_enabled:
             # this should never be triggered since this is intended for UI-disabling and the
             # UI section is hidden, but would prevent any JS-hacking
-            raise ValueError("Writing out moment map to file is currently disabled")
+            raise ValueError("Writing out collapsed cube to file is currently disabled")
 
         # Make sure file does not end up in weird places in standalone mode.
         path = os.path.dirname(self.filename)
         if path and not os.path.exists(path):
             raise ValueError(f"Invalid path={path}")
         elif (not path or path.startswith("..")) and os.environ.get("JDAVIZ_START_DIR", ""):  # noqa: E501 # pragma: no cover
             filename = Path(os.environ["JDAVIZ_START_DIR"]) / self.filename
@@ -177,12 +176,13 @@
                     # Warn the user if the file still exists
                     raise FileExistsError(f"Unable to delete {filename}. Check user permissions.")
             else:
                 self.overwrite_warn = True
                 return
 
         filename = str(filename)
-        self.moment.write(filename)
+        self.collapsed_spec.write(filename)
 
         # Let the user know where we saved the file.
         self.hub.broadcast(SnackbarMessage(
-            f"Moment map saved to {os.path.abspath(filename)}", sender=self, color="success"))
+            f"Collapsed cube saved to {os.path.abspath(filename)}",
+                           sender=self, color="success"))
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.vue` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/collapse/collapse.vue`

 * *Files 24% similar despite different names*

```diff
@@ -1,93 +1,100 @@
 <template>
   <j-tray-plugin
-    description='Create a 2D image from a data cube.'
-    :link="docs_link || 'https://jdaviz.readthedocs.io/en/'+vdocs+'/'+config+'/plugins.html#moment-maps'"
-    :popout_button="popout_button">
+    :description="docs_description || 'Collapse a spectral cube along one axis.'"
+    :link="docs_link || 'https://jdaviz.readthedocs.io/en/'+vdocs+'/'+config+'/plugins.html#collapse'"
+    :popout_button="popout_button"
+    :scroll_to.sync="scroll_to">
 
     <plugin-dataset-select
       :items="dataset_items"
       :selected.sync="dataset_selected"
       :show_if_single_entry="false"
       label="Data"
-      hint="Select the data set."
+      hint="Select the data set to collapse."
     />
 
-    <plugin-subset-select 
+    <v-row>
+      <v-select
+        :menu-props="{ left: true }"
+        attach
+        :items="function_items.map(i => i.label)"
+        v-model="function_selected"
+        label="Function"
+        hint="Function to use in the collapse."
+        persistent-hint
+      ></v-select>
+    </v-row>
+
+    <plugin-subset-select
       :items="spectral_subset_items"
       :selected.sync="spectral_subset_selected"
       :has_subregions="spectral_subset_selected_has_subregions"
       :show_if_single_entry="true"
       has_subregions_warning="The selected selected subset has subregions, the entire range will be used, ignoring any gaps."
       label="Spectral region"
-      hint="Spectral region to compute the moment map."
+      hint="Select spectral region to apply the collapse."
     />
 
-    <v-row>
-      <v-text-field
-        ref="n_moment"
-        type="number"
-        label="Moment"
-        v-model.number="n_moment"
-        hint="The desired moment."
-        persistent-hint
-        :rules="[() => n_moment !== '' || 'This field is required',
-                 () => n_moment >=0 || 'Moment must be positive']"
-      ></v-text-field>
-    </v-row>
-
     <plugin-add-results
       :label.sync="results_label"
       :label_default="results_label_default"
       :label_auto.sync="results_label_auto"
       :label_invalid_msg="results_label_invalid_msg"
       :label_overwrite="results_label_overwrite"
       label_hint="Label for the collapsed cube"
       :add_to_viewer_items="add_to_viewer_items"
       :add_to_viewer_selected.sync="add_to_viewer_selected"
-      action_label="Calculate"
-      action_tooltip="Calculate moment map"
+      action_label="Collapse"
+      action_tooltip="Collapse data"
       :action_spinner="spinner"
-      @click:action="calculate_moment"
+      @click:action="collapse"
     ></plugin-add-results>
-    
-    <j-plugin-section-header v-if="export_enabled">Results</j-plugin-section-header>
+
+    <j-plugin-section-header v-if="collapsed_spec_available && export_enabled">Results</j-plugin-section-header>
 
     <div style="display: grid; position: relative"> <!-- overlay container -->
       <div style="grid-area: 1/1">
-        <div v-if="moment_available && export_enabled">
+        <div v-if="collapsed_spec_available && export_enabled">
+
           <v-row>
-              <v-text-field
-              v-model="filename"
-              label="Filename"
-              hint="Export the latest calculated moment map"
-              :rules="[() => !!filename || 'This field is required']"
-              persistent-hint>
-              </v-text-field>
+            <v-text-field
+            v-model="filename"
+            label="Filename"
+            hint="Export the latest collapsed spectrum."
+            :rules="[() => !!filename || 'This field is required']"
+            persistent-hint>
+            </v-text-field>
+          </v-row>
+
+          <v-row>
+            <span class="v-messages v-messages__message text--secondary" style="color: red !important">
+              DeprecationWarning: Save as FITS functionality has moved to the Export plugin as of v3.9 and will be removed from here in a future release.
+            </span>
           </v-row>
 
           <v-row justify="end">
-            <j-tooltip tipid='plugin-moment-save-fits'>
+            <j-tooltip tipid='plugin-collapse-save-fits'>
               <v-btn color="primary" text @click="save_as_fits">Save as FITS</v-btn>
 
             </j-tooltip>
           </v-row>
 
         </div>
       </div>
 
       <v-overlay
         absolute
         opacity=1.0
         :value="overwrite_warn && export_enabled"
         :zIndex=3
-        style="grid-area: 1/1; 
+        style="grid-area: 1/1;
                margin-left: -24px;
                margin-right: -24px">
-      
+
       <v-card color="transparent" elevation=0 >
         <v-card-text width="100%">
           <div class="white--text">
             A file with this name is already on disk. Overwrite?
           </div>
         </v-card-text>
 
@@ -97,11 +104,10 @@
             <v-btn tile small color="accent" class="mr-4" @click="overwrite_fits" >Overwrite</v-btn>
           </v-row>
         </v-card-actions>
       </v-card>
 
       </v-overlay>
 
-
     </div>
   </j-tray-plugin>
 </template>
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/moment_maps/tests/test_moment_maps.py` & `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/moment_maps/tests/test_moment_maps.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,51 +5,86 @@
 import pytest
 from astropy.io import fits
 from astropy.nddata import CCDData
 from astropy.wcs import WCS
 from astroquery.mast import Observations
 from numpy.testing import assert_allclose
 
-from jdaviz.configs.cubeviz.plugins.moment_maps.moment_maps import MomentMap
 
+def test_user_api(cubeviz_helper, spectrum1d_cube):
+    with warnings.catch_warnings():
+        warnings.filterwarnings("ignore", message="No observer defined on WCS.*")
+        cubeviz_helper.load_data(spectrum1d_cube, data_label='test')
+
+    mm = cubeviz_helper.plugins['Moment Maps']
+    assert not mm._obj.continuum_marks['center'].visible
+    with mm.as_active():
+        assert mm._obj.continuum_marks['center'].visible
+        mm.n_moment = 0
+        # no continuum so marks should be empty
+        assert len(mm._obj.continuum_marks['center'].x) == 0
+
+        mom = mm.calculate_moment()
+
+        mm.continuum = 'Surrounding'
+        mm.continuum_width = 10
+        assert len(mm._obj.continuum_marks['center'].x) > 0
+
+        mom_sub = mm.calculate_moment()
+        assert isinstance(mom_sub.wcs, WCS)
+
+        assert mom != mom_sub
+
+        mm.n_moment = -1
+        with pytest.raises(ValueError, match="Moment must be a positive integer"):
+            mm.calculate_moment()
+
+        mm.n_moment = 1
+        with pytest.raises(ValueError, match="not one of"):
+            mm._obj.output_unit_selected = "Bad Unit"
+        mm._obj.output_unit_selected = "Flux"
+        with pytest.raises(ValueError, match="units must be in"):
+            mm.calculate_moment()
 
-def test_moment_calculation(cubeviz_helper, spectrum1d_cube, tmpdir):
+
+def test_moment_calculation(cubeviz_helper, spectrum1d_cube, tmp_path):
     dc = cubeviz_helper.app.data_collection
     with warnings.catch_warnings():
         warnings.filterwarnings("ignore", message="No observer defined on WCS.*")
         cubeviz_helper.load_data(spectrum1d_cube, data_label='test')
     flux_viewer = cubeviz_helper.app.get_viewer(cubeviz_helper._default_flux_viewer_reference_name)
 
     # Since we are not really displaying, need this to trigger GUI stuff.
     flux_viewer.shape = (100, 100)
     flux_viewer.state._set_axes_aspect_ratio(1)
 
-    mm = MomentMap(app=cubeviz_helper.app)
-    mm.dataset_selected = 'test[FLUX]'
+    mm = cubeviz_helper.plugins["Moment Maps"]
+    mm.dataset = 'test[FLUX]'
 
     mm.n_moment = 0  # Collapsed sum, will get back 2D spatial image
-    assert mm.results_label == 'moment 0'
+    assert mm._obj.results_label == 'moment 0'
+    assert mm.output_unit == "Flux"
 
-    mm.add_results.viewer.selected = cubeviz_helper._default_uncert_viewer_reference_name
-    mm.vue_calculate_moment()
+    mm._obj.add_results.viewer.selected = cubeviz_helper._default_uncert_viewer_reference_name
+    mm._obj.vue_calculate_moment()
 
-    assert mm.moment_available
+    assert mm._obj.moment_available
     assert dc[1].label == 'moment 0'
     mv_data = cubeviz_helper.app.get_viewer(
         cubeviz_helper._default_uncert_viewer_reference_name
     ).data()
     # by default, will overwrite the previous entry (so only one data entry)
     assert len(mv_data) == 1
     assert mv_data[0].label == 'moment 0'
 
     assert len(dc.links) == 14
 
     # label should remain unchanged but raise overwrite warnings
-    assert mm.results_label == 'moment 0'
-    assert mm.results_label_overwrite is True
+    assert mm._obj.results_label == 'moment 0'
+    assert mm._obj.results_label_overwrite is True
 
     # Make sure coordinate display works
     label_mouseover = cubeviz_helper.app.session.application._tools['g-coords-info']
     label_mouseover._viewer_mouse_event(flux_viewer, {'event': 'mousemove',
                                                       'domain': {'x': 0, 'y': 0}})
     assert flux_viewer.state.slices == (0, 0, 1)
     # Slice 0 has 8 pixels, this is Slice 1
@@ -71,23 +106,24 @@
                                                       'domain': {'x': 0, 'y': 0}})
 
     # Slice 0 has 8 pixels, this is Slice 1  # noqa
     assert label_mouseover.as_text() == ("Pixel x=00.0 y=00.0 Value +8.00000e+00 Jy",
                                          "World 13h39m59.9731s +27d00m00.3600s (ICRS)",
                                          "204.9998877673 27.0001000000 (deg)")
 
-    assert mm.filename == 'moment0_test_FLUX.fits'  # Auto-populated on calculate.
-    mm.filename = str(tmpdir.join(mm.filename))  # But we want it in tmpdir for testing.
-    mm.vue_save_as_fits()
-    assert os.path.isfile(mm.filename)
-
-    mm.n_moment = 1
-    assert mm.results_label == 'moment 1'
-    assert mm.results_label_overwrite is False
-    mm.vue_calculate_moment()
+    assert mm._obj.filename == 'moment0_test_FLUX.fits'  # Auto-populated on calculate.
+    mm._obj.filename = str(tmp_path / mm._obj.filename)  # But we want it in tmp_path for testing.
+    mm._obj.vue_save_as_fits()
+    assert os.path.isfile(mm._obj.filename)
+
+    mm._obj.n_moment = 1
+    mm._obj.output_unit_selected = "Spectral Unit"
+    assert mm._obj.results_label == 'moment 1'
+    assert mm._obj.results_label_overwrite is False
+    mm._obj.vue_calculate_moment()
 
     assert dc[2].label == 'moment 1'
 
     assert len(dc.links) == 22
     assert len(dc.external_links) == 4  # pixel linked
     # Link 3D z to 2D x and 3D y to 2D y
 
@@ -95,14 +131,61 @@
     label_mouseover._viewer_mouse_event(flux_viewer, {'event': 'mousemove',
                                                       'domain': {'x': 0, 'y': 0}})
     assert label_mouseover.as_text() == ("Pixel x=00.0 y=00.0 Value +8.00000e+00 Jy",
                                          "World 13h39m59.9731s +27d00m00.3600s (ICRS)",
                                          "204.9998877673 27.0001000000 (deg)")
 
 
+def test_moment_velocity_calculation(cubeviz_helper, spectrum1d_cube):
+    with warnings.catch_warnings():
+        warnings.filterwarnings("ignore", message="No observer defined on WCS.*")
+        cubeviz_helper.load_data(spectrum1d_cube, data_label='test')
+
+    uncert_viewer = cubeviz_helper.app.get_viewer("uncert-viewer")
+
+    # Since we are not really displaying, need this to trigger GUI stuff.
+    uncert_viewer.shape = (100, 100)
+    uncert_viewer.state._set_axes_aspect_ratio(1)
+
+    mm = cubeviz_helper.plugins["Moment Maps"]
+    print(mm._obj.dataset_selected)
+    mm._obj.dataset_selected = 'test[FLUX]'
+
+    # Test moment 1 in velocity
+    mm.n_moment = 1
+    mm.add_results.viewer = "uncert-viewer"
+    assert mm._obj.results_label == 'moment 1'
+    mm.output_unit = "Velocity"
+
+    with pytest.raises(ValueError, match="reference_wavelength must be set"):
+        mm.calculate_moment()
+
+    mm.reference_wavelength = 4.63e-7
+    mm.calculate_moment()
+
+    # Make sure coordinate display works
+    label_mouseover = cubeviz_helper.app.session.application._tools['g-coords-info']
+    label_mouseover._viewer_mouse_event(uncert_viewer, {'event': 'mousemove',
+                                                        'domain': {'x': 0, 'y': 0}})
+    assert label_mouseover.as_text() == ("Pixel x=00.0 y=00.0 Value -4.14668e+02 km / s",
+                                         "World 13h39m59.9731s +27d00m00.3600s (ICRS)",
+                                         "204.9998877673 27.0001000000 (deg)")
+
+    # Test moment 2 in velocity
+    mm.n_moment = 2
+    mm.calculate_moment()
+
+    label_mouseover._viewer_mouse_event(uncert_viewer, {'event': 'mousemove',
+                                                        'domain': {'x': 1, 'y': 1}})
+
+    assert label_mouseover.as_text() == ("Pixel x=01.0 y=01.0 Value +2.32415e+01 km / s",
+                                         "World 13h39m59.9461s +27d00m00.7200s (ICRS)",
+                                         "204.9997755344 27.0001999998 (deg)")
+
+
 def test_write_momentmap(cubeviz_helper, spectrum1d_cube, tmp_path):
     ''' Test writing a moment map out to a FITS file on disk '''
 
     # Simulate an existing file on disk to check for overwrite warning
     test_file = tmp_path / "test_file.fits"
     test_file_str = str(test_file)
     existing_sentinel_text = "This is a simulated, existing file on disk"
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/parsers.py` & `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/slice/slice.vue` & `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/slice/slice.vue`

 * *Files 26% similar despite different names*

```diff
@@ -1,106 +1,103 @@
 <template>
   <j-tray-plugin
-    description='Select slice (or wavelength) of the cube to show in the image viewers and highlighted in the spectrum viewer.  The slice can also be changed interactively in the spectrum viewer by activating the slice tool.'
+    :description="docs_description || 'Select slice of the cube to show in the image viewers.  The slice can also be changed interactively in the spectrum viewer by activating the slice tool.'"
+    :irrelevant_msg="irrelevant_msg"
     :link="docs_link || 'https://jdaviz.readthedocs.io/en/'+vdocs+'/'+config+'/plugins.html#slice'"
-    :popout_button="popout_button">
+    :popout_button="popout_button"
+    :scroll_to.sync="scroll_to">
 
     <v-row>
       <v-expansion-panels popout>
         <v-expansion-panel>
           <v-expansion-panel-header v-slot="{ open }">
             <span style="padding: 6px">Indicator Settings</span>
           </v-expansion-panel-header>
           <v-expansion-panel-content class="plugin-expansion-panel-content">
+            <v-row v-if="allow_disable_snapping">
+              <v-switch
+                label="Snap to Slice"
+                hint="Snap indicator (and value) to the nearest slice in the cube."
+                v-model="snap_to_slice"
+                persistent-hint>
+              </v-switch>
+            </v-row>
             <v-row>
               <v-switch
                 label="Show Indicator"
-                hint="Show indicator in spectral viewer even when slice tool is inactive."
+                hint="Show slice indicator even when slice tool is inactive."
                 v-model="show_indicator"
                 persistent-hint>
               </v-switch>
             </v-row>
             <v-row>
               <v-switch
-                label="Show Wavelength"
-                hint="Show slice wavelength in label to right of indicator."
-                v-model="show_wavelength"
+                label="Show Value"
+                :hint="'Show slice '+value_label.toLowerCase()+' in label to right of indicator.'"
+                v-model="show_value"
                 persistent-hint>
               </v-switch>
             </v-row>
           </v-expansion-panel-content>
         </v-expansion-panel>
       </v-expansion-panels>
     </v-row>
 
-    <v-row>
-      <v-slider
-        :value="slice"
-        @input="throttledSetValue"
-        class="align-center"
-        :max="max_value"
-        :min="min_value"
-        hide-details
-      />
-    </v-row>
-
-    <v-row class="row-no-outside-padding row-min-bottom-padding">
-      <v-col>
-        <v-text-field
-          v-model.number="slice"
-          class="mt-0 pt-0"
-          type="number"
-          label="Slice"
-          hint="Slice number"
-        ></v-text-field>
-      </v-col>
-      <v-col cols=3>
-        <span> / {{ max_value }}</span>
-      </v-col>
+    <v-row justify="end">
+      <v-btn color="primary" text v-if="!cube_viewer_exists" @click="create_cube_viewer">
+        Show Cube Viewer
+      </v-btn>
     </v-row>
 
-    <v-row class="row-no-outside-padding">
-      <v-col>
-        <v-text-field
-          v-model="wavelength"
-          class="mt-0 pt-0"
-          label="Wavelength"
-          hint="Wavelength corresponding to slice, in units of spectrum"
-        ></v-text-field>
-      </v-col>
-      <v-col cols=3>
-        <span>{{ wavelength_unit }}</span>
-      </v-col>
+    <v-row>
+      <v-text-field
+        type="number"
+        v-model.number="value"
+        @focus="(e) => value_editing = true"
+        @blur="(e) => value_editing = false"
+        class="mt-0 pt-0"
+        :label="value_label"
+        :hint="value_label+' corresponding to slice.'+(snap_to_slice && value_editing ? '  Indicator will snap to slice when clicking or tabbing away from input.' : '')"
+        :suffix="value_unit"
+      ></v-text-field>
     </v-row>
 
     <v-row class="row-no-outside-padding row-min-bottom-padding">
       <v-col>
         <v-tooltip top>
           <template v-slot:activator="{ on, attrs }">
             <v-btn color="primary" icon @click="goto_first" v-bind="attrs" v-on="on" :disabled="is_playing">
               <v-icon>skip_previous</v-icon>
             </v-btn>
           </template>
           <span>Jump to first</span>
         </v-tooltip>
         <v-tooltip top>
           <template v-slot:activator="{ on, attrs }">
+            <v-btn color="primary" icon @click="play_prev" v-bind="attrs" v-on="on" :disabled="is_playing">
+              <v-icon>exposure_minus_1</v-icon>
+            </v-btn>
+          </template>
+          <span>Previous</span>
+        </v-tooltip>
+        <v-tooltip top>
+          <template v-slot:activator="{ on, attrs }">
             <v-btn color="primary" icon @click="play_start_stop" v-bind="attrs" v-on="on">
               <v-icon>mdi-play-pause</v-icon>
             </v-btn>
           </template>
           <span>Play/Pause</span>
         </v-tooltip>
         <v-tooltip top>
           <template v-slot:activator="{ on, attrs }">
             <v-btn color="primary" icon @click="play_next" v-bind="attrs" v-on="on" :disabled="is_playing">
               <v-icon>exposure_plus_1</v-icon>
             </v-btn>
           </template>
-          <span>Next slice</span>
+          <span>Next</span>
         </v-tooltip>
         <v-tooltip top>
           <template v-slot:activator="{ on, attrs }">
             <v-btn color="primary" icon @click="goto_last" v-bind="attrs" v-on="on" :disabled="is_playing">
               <v-icon>skip_next</v-icon>
             </v-btn>
           </template>
@@ -112,15 +109,15 @@
 </template>
 
 <script>
   module.exports = {
     created() {
       this.throttledSetValue = _.throttle(
         (v) => { this.slice = v; },
-        this.wait);
+        this.slider_throttle);
     },
   }
 </script>
 
 <style>
   .v-slider {
     margin: 0px !important;
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/slice/tests/test_slice.py` & `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/slice/tests/test_slice.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,94 +1,77 @@
 import warnings
 
 import pytest
-import numpy as np
 
 from jdaviz.configs.cubeviz.plugins.slice.slice import Slice
 
 
 def test_slice(cubeviz_helper, spectrum1d_cube):
     app = cubeviz_helper.app
     sl = Slice(app=app)
 
-    # Make sure nothing crashes if plugin used without data
+    # No data yet
+    assert len(sl.slice_selection_viewers) == 2  # flux-viewer, uncert-viewer
+    assert len(sl.slice_indicator_viewers) == 1  # spectrum-viewer
+    assert len(sl.valid_indicator_values_sorted) == 0
+    assert len(sl.valid_selection_values_sorted) == 0
+
+    # Make sure nothing crashes if plugin used without data]
     sl.vue_play_next()
-    assert sl.slice == 0
     sl.vue_play_start_stop()
     assert not sl.is_playing
-    assert not sl._player
 
-    app.add_data(spectrum1d_cube, 'test')
-    app.add_data_to_viewer("spectrum-viewer", "test")
-    app.add_data_to_viewer("flux-viewer", "test")
-    app.add_data_to_viewer("uncert-viewer", "test")
+    cubeviz_helper.load_data(spectrum1d_cube, data_label='test')
+    app.add_data_to_viewer("spectrum-viewer", "test[FLUX]")
+    app.add_data_to_viewer("flux-viewer", "test[FLUX]")
+    app.add_data_to_viewer("uncert-viewer", "test[FLUX]")
 
     # sample cube only has 2 slices with wavelengths [4.62280007e-07 4.62360028e-07] m
-    assert sl.slice == 1
+    assert len(sl.valid_indicator_values_sorted) == 2
+    slice_values = sl.valid_selection_values_sorted
+    assert len(slice_values) == 2
+
+    assert sl.value == slice_values[1]
+    assert cubeviz_helper.app.get_viewer("flux-viewer").slice == 1
     assert cubeviz_helper.app.get_viewer("flux-viewer").state.slices[-1] == 1
     assert cubeviz_helper.app.get_viewer("uncert-viewer").state.slices[-1] == 1
-    cubeviz_helper.select_slice(0)
-    assert sl.slice == 0
+    cubeviz_helper.select_wavelength(slice_values[0])
+    assert cubeviz_helper.app.get_viewer("flux-viewer").slice == 0
+    assert sl.value == slice_values[0]
 
-    with pytest.raises(
-            TypeError,
-            match="slice must be an integer"):
-        cubeviz_helper.select_slice("blah")
-
-    with pytest.raises(
-            ValueError,
-            match="slice must be positive"):
-        cubeviz_helper.select_slice(-5)
-
-    cubeviz_helper.select_wavelength(4.62360028e-07)
-    assert sl.slice == 1
-
-    # from the widget this logic is duplicated (to avoid sending logic through messages)
-    sl._on_wavelength_updated({'new': '4.62e-07'})
-    assert sl.slice == 0
-    assert np.allclose(sl.wavelength, 4.62280007e-07)
-
-    # make sure that passing an invalid value from the UI would revert to the previous value
-    # JS strips invalid characters, but doesn't ensure its float-compatible
-    sl._on_wavelength_updated({'new': '1.2.3'})
-    assert sl.slice == 0
-
-    assert len(sl._watched_viewers) == 2  # flux-viewer, uncert-viewer
-    assert len(sl._indicator_viewers) == 1  # spectrum-viewer
+    cubeviz_helper.select_wavelength(slice_values[1])
+    assert sl.value == slice_values[1]
 
     # test setting a static 2d image to the "watched" flux viewer to make sure it disconnects
     mm = app.get_tray_item_from_name('cubeviz-moment-maps')
     mm.add_to_viewer_selected = 'flux-viewer'
     with warnings.catch_warnings():
         warnings.filterwarnings('ignore', message=r'.*No observer defined on WCS.*')
         mm.vue_calculate_moment()
 
-    assert len(sl._watched_viewers) == 2
-    assert len(sl._indicator_viewers) == 1
-
     # test in conjunction with as_steps
     sv = app.get_viewer('spectrum-viewer')
     orig_len = len(sv.native_marks[0].x)
 
     sv.state.layers[0].as_steps = True
     new_len = len(sv.native_marks[0].x)
     assert new_len == 2*orig_len
     cubeviz_helper.select_wavelength(4.62360028e-07)
-    assert sl.slice == 1
+    assert sl.value == slice_values[1]
 
     # Test player buttons API
 
     sl.vue_goto_first()
-    assert sl.slice == 0
+    assert sl.value == slice_values[0]
 
     sl.vue_goto_last()
-    assert sl.slice == sl.max_value
+    assert sl.value == slice_values[-1]
 
     sl.vue_play_next()  # Should automatically wrap to beginning
-    assert sl.slice == 0
+    assert sl.value == slice_values[0]
 
     sl.vue_play_start_stop()  # Start
     assert sl.is_playing
     assert sl._player.is_alive()
     sl.vue_play_next()  # Should be no-op
     sl.vue_goto_last()  # Should be no-op
     sl.vue_goto_first()  # Should be no-op
@@ -105,32 +88,36 @@
     app.add_data_to_viewer("flux-viewer", "test")
     sl = Slice(app=app)
     sv = app.get_viewer('spectrum-viewer')
     indicator = sv.slice_indicator
 
     assert sl.show_indicator is True
     assert indicator._show_if_inactive is True
-    assert sl.show_wavelength is True
+    assert sl.show_value is True
     assert indicator.label.visible is True
 
     sl.show_indicator = False
     assert indicator._show_if_inactive is False
 
-    sl.show_wavelength = False
+    sl.show_value = False
     assert indicator.label.visible is False
 
 
 @pytest.mark.filterwarnings('ignore:No observer defined on WCS')
 def test_init_slice(cubeviz_helper, spectrum1d_cube):
     cubeviz_helper.load_data(spectrum1d_cube, data_label='test')
 
     fv = cubeviz_helper.app.get_viewer('flux-viewer')
     sl = cubeviz_helper.plugins['Slice']
-    assert sl.slice == 1
+    slice_values = sl._obj.valid_selection_values_sorted
+
+    assert sl.value == slice_values[1]
+    assert fv.slice == 1
     assert fv.state.slices == (0, 0, 1)
 
     # make sure adding new data doesn't revert slice to 0
     mm = cubeviz_helper.plugins['Moment Maps']
     mm.calculate_moment(add_data=True)
 
-    assert sl.slice == 1
+    assert sl.value == slice_values[1]
+    assert fv.slice == 1
     assert fv.state.slices == (0, 0, 1)
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/tests/test_cubeviz_helper.py` & `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_cubeviz_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,21 @@
     assert spec_viewer.jdaviz_helper == cubeviz_helper
 
 
 def test_plugin_user_apis(cubeviz_helper):
     for plugin_name, plugin_api in cubeviz_helper.plugins.items():
         plugin = plugin_api._obj
         for attr in plugin_api._expose:
+            if plugin_name == 'Spectral Extraction' and attr == 'spatial_subset':
+                # deprecated, so would raise a deprecation warning
+                continue
+            if plugin_name == 'Slice' and attr in ('slice', 'wavelength',
+                                                   'wavelength_unit', 'show_wavelength'):
+                # deprecated, so would raise a deprecation warning
+                continue
             assert hasattr(plugin, attr)
 
 
 def test_invalid_function(cubeviz_helper, spectrum1d_cube):
     cubeviz_helper.load_data(spectrum1d_cube, "test")
     cubeviz_helper._apply_interactive_region('bqplot:ellipse', (0, 0), (9, 8))
 
@@ -75,16 +82,16 @@
 
 def test_remote_server_disable_save_serverside():
     config = get_configuration('cubeviz')
     config['settings']['server_is_remote'] = True
 
     cubeviz_app = Application(config)
     cubeviz_helper = Cubeviz(cubeviz_app)
-    ep = cubeviz_helper.plugins['Export Plot']
-    assert ep._obj.movie_enabled is False
+    exp = cubeviz_helper.plugins['Export']
+    assert 'mp4' not in exp.viewer_format.choices
 
     mm = cubeviz_helper.plugins['Moment Maps']
     assert mm._obj.export_enabled is False
 
 
 def test_get_data_spatial_and_spectral(cubeviz_helper, spectrum1d_cube_larger):
     data_label = "test"
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/tests/test_data_retrieval.py` & `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_data_retrieval.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/tests/test_data_selection.py` & `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_data_selection.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/tests/test_parsers.py` & `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     label_mouseover = cubeviz_helper.app.session.application._tools['g-coords-info']
     label_mouseover._viewer_mouse_event(flux_viewer,
                                         {'event': 'mousemove', 'domain': {'x': 0, 'y': 0}})
     if ASTROPY_LT_5_3:
         flux_unit_str = "erg / (Angstrom cm2 s)"
     else:
         flux_unit_str = "erg / (Angstrom s cm2)"
-    assert label_mouseover.as_text() == (f'Pixel x=00.0 y=00.0 Value +1.00000e+00 1e-17 {flux_unit_str}',  # noqa
+    assert label_mouseover.as_text() == (f'Pixel x=00.0 y=00.0 Value +5.00000e+00 1e-17 {flux_unit_str}',  # noqa
                                          'World 13h41m45.5759s +27d00m12.3044s (ICRS)',
                                          '205.4398995981 27.0034178810 (deg)')  # noqa
     unc_viewer = cubeviz_helper.app.get_viewer('uncert-viewer')
     label_mouseover._viewer_mouse_event(unc_viewer,
                                         {'event': 'mousemove', 'domain': {'x': -1, 'y': 0}})
     assert label_mouseover.as_text() == ('Pixel x=-1.0 y=00.0',  # Out of bounds
                                          'World 13h41m45.5856s +27d00m12.3044s (ICRS)',
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/tests/test_regions.py` & `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_regions.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 from jdaviz.configs.imviz.tests.test_regions import BaseRegionHandler
 
 
 class TestLoadRegions(BaseRegionHandler):
     @pytest.fixture(autouse=True)
     def setup_class(self, cubeviz_helper, image_cube_hdu_obj_microns):
-        cubeviz_helper.load_data(image_cube_hdu_obj_microns, data_label='has_microns')
         self.cubeviz = cubeviz_helper
+        cubeviz_helper.load_data(image_cube_hdu_obj_microns, data_label='has_microns')
         self.viewer = cubeviz_helper.default_viewer._obj  # This is used in BaseRegionHandler
         self.spectrum_viewer = cubeviz_helper.app.get_viewer(
             cubeviz_helper._default_spectrum_viewer_reference_name
         )
 
     def teardown_method(self, method):
         """Clear all the subsets for the next test method."""
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/tests/test_tools.py` & `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/tests/test_tools.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,104 @@
 import pytest
 from astropy.nddata import CCDData
 from echo import delay_callback
 from regions import RectanglePixelRegion
 
 
 @pytest.mark.filterwarnings('ignore:No observer defined on WCS')
-def test_spectrum_at_spaxel(cubeviz_helper, spectrum1d_cube):
-    cubeviz_helper.load_data(spectrum1d_cube, data_label='test')
+def test_spectrum_at_spaxel(cubeviz_helper, spectrum1d_cube_with_uncerts):
+    cubeviz_helper.load_data(spectrum1d_cube_with_uncerts, data_label='test')
 
     flux_viewer = cubeviz_helper.app.get_viewer("flux-viewer")
+    uncert_viewer = cubeviz_helper.app.get_viewer("uncert-viewer")
     spectrum_viewer = cubeviz_helper.app.get_viewer("spectrum-viewer")
 
     # Set the active tool to spectrumperspaxel
     flux_viewer.toolbar.active_tool = flux_viewer.toolbar.tools['jdaviz:spectrumperspaxel']
     x = 1
     y = 1
     assert len(flux_viewer.native_marks) == 2
     assert len(spectrum_viewer.data()) == 1
 
+    # Move to spaxel location
+    flux_viewer.toolbar.active_tool.on_mouse_move(
+        {'event': 'mousemove', 'domain': {'x': x, 'y': y}, 'altKey': False})
+    assert flux_viewer.toolbar.active_tool._mark in spectrum_viewer.figure.marks
+    assert flux_viewer.toolbar.active_tool._mark.visible is True
+
     # Click on spaxel location
     flux_viewer.toolbar.active_tool.on_mouse_event(
         {'event': 'click', 'domain': {'x': x, 'y': y}, 'altKey': False})
     assert len(flux_viewer.native_marks) == 3
     assert len(spectrum_viewer.data()) == 2
 
     # Check that a new subset was created
     subsets = cubeviz_helper.app.get_subsets()
     reg = subsets.get('Subset 1')[0]['region']
     assert len(subsets) == 1
     assert isinstance(reg, RectanglePixelRegion)
 
+    # Move out of bounds
+    flux_viewer.toolbar.active_tool.on_mouse_move(
+        {'event': 'mousemove', 'domain': {'x': -1, 'y': -1}, 'altKey': False})
+    assert flux_viewer.toolbar.active_tool._mark.visible is False
+
+    # Mouse leave event
+    flux_viewer.toolbar.active_tool.on_mouse_move(
+        {'event': 'mouseleave', 'domain': {'x': x, 'y': y}, 'altKey': False})
+    assert flux_viewer.toolbar.active_tool._mark.visible is False
+
     # Deselect tool
     flux_viewer.toolbar.active_tool = None
     assert len(flux_viewer.native_marks) == 3
 
+    # Check in uncertainty viewer as well. Set mouseover here
+    cubeviz_helper.app.session.application._tools['g-coords-info'].dataset.selected = 'none'
+    uncert_viewer.toolbar.active_tool = uncert_viewer.toolbar.tools['jdaviz:spectrumperspaxel']
+    uncert_viewer.toolbar.active_tool.on_mouse_move(
+        {'event': 'mousemove', 'domain': {'x': x, 'y': y}, 'altKey': False})
+    assert uncert_viewer.toolbar.active_tool._mark in spectrum_viewer.figure.marks
+    assert uncert_viewer.toolbar.active_tool._mark.visible is True
+
+    # Select specific data
+    cubeviz_helper.app.session.application._tools['g-coords-info'].dataset.selected = 'test[FLUX]'
+    uncert_viewer.toolbar.active_tool = uncert_viewer.toolbar.tools['jdaviz:spectrumperspaxel']
+    uncert_viewer.toolbar.active_tool.on_mouse_move(
+        {'event': 'mousemove', 'domain': {'x': x, 'y': y}, 'altKey': False})
+    assert uncert_viewer.toolbar.active_tool._mark in spectrum_viewer.figure.marks
+    assert uncert_viewer.toolbar.active_tool._mark.visible is True
+
 
 def test_spectrum_at_spaxel_altkey_true(cubeviz_helper, spectrum1d_cube):
     cubeviz_helper.load_data(spectrum1d_cube, data_label='test')
 
     flux_viewer = cubeviz_helper.app.get_viewer("flux-viewer")
     uncert_viewer = cubeviz_helper.app.get_viewer("uncert-viewer")
     spectrum_viewer = cubeviz_helper.app.get_viewer("spectrum-viewer")
 
     # Set the active tool to spectrumperspaxel
     flux_viewer.toolbar.active_tool = flux_viewer.toolbar.tools['jdaviz:spectrumperspaxel']
-    x = 1
-    y = 1
+
     assert len(flux_viewer.native_marks) == 2
     assert len(spectrum_viewer.data()) == 1
 
     # Check coordinate info panel
+    sl = cubeviz_helper.plugins['Slice']
+    sl.value = sl._obj.valid_indicator_values_sorted[1]
+    assert flux_viewer.slice == 1
     label_mouseover = cubeviz_helper.app.session.application._tools['g-coords-info']
     label_mouseover._viewer_mouse_event(flux_viewer,
                                         {'event': 'mousemove', 'domain': {'x': 1, 'y': 1}})
     assert label_mouseover.as_text() == ('Pixel x=01.0 y=01.0 Value +1.30000e+01 Jy',
                                          'World 13h39m59.9461s +27d00m00.7200s (ICRS)',
                                          '204.9997755344 27.0001999998 (deg)')
 
     # Click on spaxel location
+    x = 1
+    y = 1
     flux_viewer.toolbar.active_tool.on_mouse_event(
         {'event': 'click', 'domain': {'x': x, 'y': y}, 'altKey': False})
     assert len(flux_viewer.native_marks) == 3
     assert len(spectrum_viewer.data()) == 2
 
     # Check that subset was created
     subsets = cubeviz_helper.app.get_subsets()
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/cubeviz/plugins/viewers.py` & `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/viewers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,145 @@
+import numpy as np
+
+from functools import cached_property
 from glue.core import BaseData
 
 from glue.core.subset_group import GroupedSubset
 from bqplot import Lines
 from glue_jupyter.bqplot.image import BqplotImageView
 
 from jdaviz.core.registries import viewer_registry
 from jdaviz.core.marks import SliceIndicatorMarks, ShadowSpatialSpectral
 from jdaviz.configs.cubeviz.helper import layer_is_cube_image_data
 from jdaviz.configs.default.plugins.viewers import JdavizViewerMixin
 from jdaviz.configs.specviz.plugins.viewers import SpecvizProfileView
-from jdaviz.utils import get_subset_type
 from jdaviz.core.events import AddDataMessage, RemoveDataMessage
+from jdaviz.core.freezable_state import FreezableBqplotImageViewerState
+from jdaviz.utils import get_subset_type
+
+__all__ = ['CubevizImageView', 'CubevizProfileView',
+           'WithSliceIndicator', 'WithSliceSelection']
+
+
+class WithSliceIndicator:
+    @property
+    def slice_component_label(self):
+        return str(self.state.x_att)
+
+    @cached_property
+    def slice_indicator(self):
+        # SliceIndicatorMarks does not yet exist
+        slice_indicator = SliceIndicatorMarks(self)
+        self.figure.marks = self.figure.marks + slice_indicator.marks
+        return slice_indicator
+
+    @property
+    def slice_values(self):
+        def _get_component(layer):
+            try:
+                return layer.layer.get_component(self.slice_component_label).data
+            except (AttributeError, KeyError):
+                # layer either does not have get_component (because its a subset)
+                # or slice_component_label is not a component in this layer
+                # either way, return an empty array and skip this layer
+                return np.array([])
+        try:
+            return np.asarray(np.unique(np.concatenate([_get_component(layer) for layer in self.layers])),  # noqa
+                              dtype=float)
+        except ValueError:
+            return np.array([])
+
+    def _set_slice_indicator_value(self, value):
+        # this is a separate method so that viewers can override and map value if necessary
+        # NOTE: on first call, this will initialize the indicator itself
+        self.slice_indicator.value = value
 
-__all__ = ['CubevizImageView', 'CubevizProfileView']
+
+class WithSliceSelection:
+    @property
+    def slice_index(self):
+        # index in state.slices corresponding to the slice axis
+        return 2
+
+    @property
+    def slice_component_label(self):
+        slice_plg = self.jdaviz_helper.plugins.get('Slice', None)
+        if slice_plg is None:  # pragma: no cover
+            raise ValueError("slice plugin must be activated to access slice_component_label")
+        return slice_plg._obj.slice_indicator_viewers[0].slice_component_label
+
+    @property
+    def slice_values(self):
+        # TODO: make a cached property and invalidate cache on add/remove data
+        # TODO: add support for multiple cubes (but then slice selection needs to be more complex)
+        # if slice_index is 0, then we want the equivalent of [:, 0, 0]
+        # if slice_index is 1, then we want the equivalent of [0, :, 0]
+        # if slice_index is 2, then we want the equivalent of [0, 0, :]
+        take_inds = [2, 1, 0]
+        take_inds.remove(self.slice_index)
+        for layer in self.layers:
+            try:
+                data_obj = layer.layer.data.get_component(self.slice_component_label).data
+            except (AttributeError, KeyError):
+                continue
+            else:
+                break
+        else:
+            return np.array([])
+        return np.asarray(data_obj.take(0, take_inds[0]).take(0, take_inds[1]), dtype=float)
+
+    @property
+    def slice(self):
+        return self.state.slices[self.slice_index]
+
+    @slice.setter
+    def slice(self, slice):
+        # NOTE: not intended for user-access - this should be controlled through the slice plugin
+        # in order to sync with all other viewers/slice indicators
+        slices = [0, 0, 0]
+        slices[self.slice_index] = slice
+        self.state.slices = tuple(slices)
+
+    @property
+    def slice_value(self):
+        return self.slice_values[self.slice]
+
+    @slice_value.setter
+    def slice_value(self, slice_value):
+        # NOTE: not intended for user-access - this should be controlled through the slice plugin
+        # in order to sync with all other viewers/slice indicators
+        # find the slice nearest slice_value
+        slice_values = self.slice_values
+        if not len(slice_values):
+            return
+        self.slice = np.argmin(abs(slice_values - slice_value))
 
 
 @viewer_registry("cubeviz-image-viewer", label="Image 2D (Cubeviz)")
-class CubevizImageView(JdavizViewerMixin, BqplotImageView):
+class CubevizImageView(JdavizViewerMixin, WithSliceSelection, BqplotImageView):
     # categories: zoom resets, (zoom, pan), subset, select tools, shortcuts
     # NOTE: zoom and pan are merged here for space consideration and to avoid
     # overflow to second row when opening the tray
     tools_nested = [
                     ['jdaviz:homezoom', 'jdaviz:prevzoom'],
                     ['jdaviz:pixelboxzoommatch', 'jdaviz:boxzoom',
                      'jdaviz:pixelpanzoommatch', 'jdaviz:panzoom'],
                     ['bqplot:truecircle', 'bqplot:rectangle', 'bqplot:ellipse',
                      'bqplot:circannulus'],
                     ['jdaviz:spectrumperspaxel'],
                     ['jdaviz:sidebar_plot', 'jdaviz:sidebar_export']
                 ]
 
     default_class = None
+    _state_cls = FreezableBqplotImageViewerState
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
+        # provide reference from state back to viewer to use for zoom syncing
+        self.state._viewer = self
 
         self._subscribe_to_layers_update()
         self.state.add_callback('reference_data', self._initial_x_axis)
 
         # Hide axes by default
         self.state.show_axes = False
 
@@ -92,15 +194,15 @@
         return [layer_state.layer  # .get_object(cls=cls or self.default_class)
                 for layer_state in self.state.layers
                 if hasattr(layer_state, 'layer') and
                 isinstance(layer_state.layer, BaseData)]
 
 
 @viewer_registry("cubeviz-profile-viewer", label="Profile 1D (Cubeviz)")
-class CubevizProfileView(SpecvizProfileView):
+class CubevizProfileView(SpecvizProfileView, WithSliceIndicator):
     # categories: zoom resets, zoom, pan, subset, select tools, shortcuts
     tools_nested = [
                     ['jdaviz:homezoom', 'jdaviz:prevzoom'],
                     ['jdaviz:boxzoom', 'jdaviz:xrangezoom', 'jdaviz:yrangezoom'],
                     ['jdaviz:panzoom', 'jdaviz:panzoom_x', 'jdaviz:panzoom_y'],
                     ['bqplot:xrange'],
                     ['jdaviz:selectslice', 'jdaviz:selectline'],
@@ -265,21 +367,7 @@
                 if _is_unique(new_shadow):
                     new_marks.append(new_shadow)
 
         else:
             return
         # NOTE: += or append won't pick up on change
         self.figure.marks = self.figure.marks + new_marks
-
-    @property
-    def slice_indicator(self):
-        for mark in self.figure.marks:
-            if isinstance(mark, SliceIndicatorMarks):
-                return mark
-
-        # SliceIndicatorMarks does not yet exist
-        slice_indicator = SliceIndicatorMarks(self)
-        self.figure.marks = self.figure.marks + slice_indicator.marks
-        return slice_indicator
-
-    def _update_slice_indicator(self, slice):
-        self.slice_indicator.slice = slice
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/default.ipynb` & `jdaviz-3.9.0/jdaviz/configs/default/default.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/data_tools/data_tools.py` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/data_tools/data_tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/data_tools/data_tools.vue` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/data_tools/data_tools.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/data_tools/file_chooser.py` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/data_tools/file_chooser.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.py` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     mode_items = List().tag(sync=True)
     mode_selected = Unicode().tag(sync=True)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         if self.config == "cubeviz":
+            self.docs_description = 'Smooth data cube spatially or spectrally with a Gaussian kernel.'  # noqa
             self.show_modes = True
             # retrieve the data from the cube, not the collapsed 1d spectrum
             self.dataset._viewers = [
                 self._default_flux_viewer_reference_name,
                 self._default_spectrum_viewer_reference_name
             ]
             # clear the cache in case the spectrum-viewer selection was already cached
@@ -210,26 +211,29 @@
         the app, set label options and use :meth:`smooth` instead.
 
         Returns
         -------
         cube : `~specutils.Spectrum1D`
             The smoothed cube
         """
-        # Get information from the flux component
-        attribute = self.dataset.selected_dc_item.main_components[0]
-
-        cube = self.dataset.get_object(cls=Spectrum1D,
-                                       attribute=attribute,
-                                       statistic=None)
+        cube = self.dataset.selected_obj
         flux_unit = cube.flux.unit
 
         # Extend the 2D kernel to have a length 1 spectral dimension, so that
         # we can do "3d" convolution to the whole cube
         kernel = np.expand_dims(Gaussian2DKernel(self.stddev), 2)
 
         convolved_data = convolve(cube, kernel)
 
+        # Copy 3D WCS from input cube.
+        data = self.dataset.selected_dc_item
+        # Similar to coords_info logic.
+        if '_orig_spec' in getattr(data, 'meta', {}):
+            w = data.meta['_orig_spec'].wcs
+        else:
+            w = data.coords
+
         # Create a new cube with the old metadata. Note that astropy
         # convolution generates values for masked (NaN) data.
-        newcube = Spectrum1D(flux=convolved_data * flux_unit, wcs=cube.wcs)
+        newcube = Spectrum1D(flux=convolved_data * flux_unit, wcs=w)
 
         return newcube
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.vue` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.vue`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 <template>
   <j-tray-plugin
-    :description="config==='cubeviz' ? 'Smooth data cube spatially or spectrally with a Gaussian kernel.' : 'Smooth data with a Gaussian kernel.'"
+    :description="docs_description || 'Smooth data with a Gaussian kernel.'"
     :link="docs_link || 'https://jdaviz.readthedocs.io/en/'+vdocs+'/'+config+'/plugins.html#gaussian-smooth'"
-    :popout_button="popout_button">
+    :popout_button="popout_button"
+    :scroll_to.sync="scroll_to">
 
       <!-- for mosviz, the entries change on row change, so we want to always show the dropdown
            to make sure that is clear -->
       <plugin-dataset-select
         :items="dataset_items"
         :selected.sync="dataset_selected"
         :show_if_single_entry="config=='mosviz'"
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/gaussian_smooth/tests/test_gaussian_smooth.py` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/gaussian_smooth/tests/test_gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/line_lists/line_list_mixin.py` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/line_lists/line_list_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,25 +38,25 @@
 
     def erase_spectral_lines(self, name=None):
         """Convenience function to get to the viewer function"""
         self.app.get_viewer(
             self._default_spectrum_viewer_reference_name
         ).erase_spectral_lines(name=name)
 
-    def plot_spectral_line(self, line):
+    def plot_spectral_line(self, line, global_redshift=None):
         """Convenience function to get to the viewer function"""
         self.app.get_viewer(
             self._default_spectrum_viewer_reference_name
-        ).plot_spectral_line(line)
+        ).plot_spectral_line(line, global_redshift)
 
-    def plot_spectral_lines(self):
+    def plot_spectral_lines(self, global_redshift=None):
         """Convenience function to get to the viewer function"""
         self.app.get_viewer(
             self._default_spectrum_viewer_reference_name
-        ).plot_spectral_lines()
+        ).plot_spectral_lines(global_redshift)
 
     @property
     def spectral_lines(self):
         return self.app.get_viewer(
             self._default_spectrum_viewer_reference_name
         ).spectral_lines
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/line_lists/line_lists.py` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/line_lists/line_lists.py`

 * *Files 1% similar despite different names*

```diff
@@ -520,15 +520,15 @@
                          "name_rest": row["name_rest"]}
             list_contents[row["listname"]]["lines"].append(temp_dict)
             tmp_names_rest.append(row["name_rest"])
 
         self.send_state('loaded_lists')
         self.send_state('list_contents')
 
-        self._viewer.plot_spectral_lines(tmp_names_rest)
+        self._viewer.plot_spectral_lines(tmp_names_rest, global_redshift=self._global_redshift)
         self.update_line_mark_dict()
 
         msg_text = ("Spectral lines loaded from notebook. Lines can be hidden"
                     "/shown in the Line Lists plugin")
         lines_loaded_message = SnackbarMessage(msg_text, sender=self,
                                                color="success", timeout=15000)
         self.hub.broadcast(lines_loaded_message)
@@ -660,15 +660,15 @@
         for line in lc[listname]["lines"]:
             line["show"] = True
             self._viewer.spectral_lines.loc[line["name_rest"]]["show"] = True
 
         self.list_contents = lc
         self.send_state('list_contents')
 
-        self._viewer.plot_spectral_lines()
+        self._viewer.plot_spectral_lines(global_redshift=self._global_redshift)
         self.update_line_mark_dict()
 
     def vue_hide_all_in_list(self, listname):
         """
         Toggle all lines in list to be hidden
         """
         name_rests = []
@@ -693,15 +693,15 @@
         for listname in self.list_contents:
             for line in self.list_contents[listname]["lines"]:
                 line["show"] = True
         self._viewer.spectral_lines["show"] = True
 
         self.send_state('list_contents')
 
-        self._viewer.plot_spectral_lines()
+        self._viewer.plot_spectral_lines(global_redshift=self._global_redshift)
         self.update_line_mark_dict()
 
     def vue_erase_all_lines(self, event):
         """
         Erase all lines from the viewer
         """
         if self._viewer.spectral_lines is None:
@@ -731,15 +731,15 @@
         if not show:
             # then make sure to also disable the identify flag
             list_contents[listname]['lines'][line_ind]['identify'] = False
         self.list_contents = {}
         self.list_contents = list_contents
 
         if show:
-            self._viewer.plot_spectral_line(name_rest)
+            self._viewer.plot_spectral_line(name_rest, global_redshift=self._global_redshift)
         else:
             self._viewer.erase_spectral_lines(name_rest=name_rest)
 
         self.update_line_mark_dict()
 
     def _update_identify_to_line(self, name_rest, listname=None, identify=True):
         list_contents = self.list_contents
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/line_lists/line_lists.vue` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/line_lists/line_lists.vue`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 <template>
   <j-tray-plugin
-    description='Plot lines from preset or custom line lists.'
+    :description="docs_description || 'Plot lines from preset or custom line lists.'"
     :link="docs_link || 'https://jdaviz.readthedocs.io/en/'+vdocs+'/'+config+'/plugins.html#line-lists'"
     :disabled_msg="disabled_msg"
-    :popout_button="popout_button">
+    :popout_button="popout_button"
+    :scroll_to.sync="scroll_to">
 
     <j-plugin-section-header>Identified Line</j-plugin-section-header>
     <v-row>
       <j-docs-link>Highlight a line and identify its name by using the line selection tool in the spectrum viewer.</j-docs-link>
     </v-row>
     <v-row v-if="rs_enabled">
       <j-tooltip v-if='identify_label' tipid='plugin-line-lists-line-identify-chip-active'>
@@ -26,15 +27,15 @@
     </v-row>
 
     <j-plugin-section-header>Redshift</j-plugin-section-header>
     <v-row>
       <j-docs-link>Shift spectral lines according to a specific redshift. Only enabled if at least one line is plotted.</j-docs-link>
     </v-row>
     <v-row style='margin-bottom: 0px'>
-      <!-- colors are app.vue primary and toolbar colors -->
+      <!-- colors are main_style.vue primary and toolbar colors -->
       <v-slider
         :value="rs_slider"
         @input="throttledSlider"
         @end="slider_reset"
         class="align-center"
         :max="rs_slider_half_range"
         :min="-rs_slider_half_range"
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/markers/markers.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,157 +1,154 @@
 import numpy as np
-from traitlets import Bool, observe
+from traitlets import Bool, Unicode, observe
 
+from jdaviz.configs.imviz.helper import get_top_layer_index
+from jdaviz.core.custom_traitlets import FloatHandleEmpty
 from jdaviz.core.events import ViewerAddedMessage
-from jdaviz.core.marks import MarkersMark
 from jdaviz.core.registries import tray_registry
-from jdaviz.core.template_mixin import PluginTemplateMixin, ViewerSelectMixin, TableMixin
-from jdaviz.core.user_api import PluginUserApi
+from jdaviz.core.template_mixin import (PluginTemplateMixin, ViewerSelectMixin, Plot,
+                                        skip_if_no_updates_since_last_active)
 
-__all__ = ['Markers']
+__all__ = ['LineProfileXY']
 
 
-@tray_registry('g-markers', label="Markers")
-class Markers(PluginTemplateMixin, ViewerSelectMixin, TableMixin):
-    """
-    See the :ref:`Markers Plugin Documentation <markers-plugin>` for more details.
-
-    Only the following attributes and methods are available through the
-    :ref:`public plugin API <plugin-apis>`:
-
-    * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.show`
-    * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.open_in_tray`
-    * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.close_in_tray`
-    * :meth:`clear_table`
-    * :meth:`~jdaviz.core.template_mixin.TableMixin.export_table`
-    """
-    template_file = __file__, "markers.vue"
+@tray_registry('imviz-line-profile-xy', label="Imviz Line Profiles (XY)")
+class LineProfileXY(PluginTemplateMixin, ViewerSelectMixin):
+    template_file = __file__, "line_profile_xy.vue"
     uses_active_status = Bool(True).tag(sync=True)
 
-    _default_table_values = {'spectral_axis': np.nan,
-                             'spectral_axis:unit': '',
-                             'slice': np.nan,
-                             'pixel': (np.nan, np.nan),
-                             'pixel:unreliable': None,
-                             'world': (np.nan, np.nan),
-                             'world:unreliable': None,
-                             'value': np.nan,
-                             'value:unit': '',
-                             'value:unreliable': None,
-                             'index': np.nan}
-
-    @property
-    def user_api(self):
-        return PluginUserApi(self, expose=('clear_table', 'export_table',))
+    plot_available = Bool(False).tag(sync=True)
+    selected_x = FloatHandleEmpty('').tag(sync=True)
+    selected_y = FloatHandleEmpty('').tag(sync=True)
+
+    plot_across_x_widget = Unicode().tag(sync=True)
+    plot_across_y_widget = Unicode().tag(sync=True)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        if self.config == 'cubeviz':
-            headers = ['spectral_axis', 'spectral_axis:unit',
-                       'slice', 'pixel',
-                       'world', 'value', 'value:unit', 'viewer']
-
-        elif self.config == 'imviz':
-            headers = ['pixel', 'pixel:unreliable',
-                       'world', 'world:unreliable',
-                       'value', 'value:unit', 'value:unreliable',
-                       'viewer']
-
-        elif self.config == 'specviz':
-            headers = ['spectral_axis', 'spectral_axis:unit',
-                       'index', 'value', 'value:unit']
-        elif self.config == 'specviz2d':
-            # TODO: add "index" if/when specviz2d supports plotting spectral_axis
-            headers = ['spectral_axis', 'spectral_axis:unit',
-                       'pixel', 'value', 'value:unit', 'viewer']
-        elif self.config == 'mosviz':
-            headers = ['spectral_axis', 'spectral_axis:unit',
-                       'pixel', 'world', 'index', 'value', 'value:unit',
-                       'viewer']
-        else:
-            # allow downstream configs to override headers
-            headers = kwargs.get('headers', [])
 
-        headers += ['data_label']
+        self.plot_across_x = Plot(self, name='across_x')
+        self.plot_across_y = Plot(self, name='across_y')
+        for plot in (self.plot_across_x, self.plot_across_y):
+            # override default styling
+            plot.figure.fig_margin = {'top': 60, 'bottom': 60, 'left': 65, 'right': 15}
+            plot.viewer.axis_x.num_ticks = 5
+            plot.viewer.axis_y.tick_format = '0.2e'
+            plot.viewer.axis_y.label_offset = '55px'
 
-        self.table.headers_avail = headers
-        self.table.headers_visible = headers
-        self.table._default_values_by_colname = self._default_table_values
+        self.plot_across_x_widget = 'IPY_MODEL_'+self.plot_across_x.model_id
+        self.plot_across_y_widget = 'IPY_MODEL_'+self.plot_across_y.model_id
 
-        # subscribe to mouse events on any new viewers
         self.hub.subscribe(self, ViewerAddedMessage, handler=self._on_viewer_added)
 
+    def reset_results(self):
+        self.plot_available = False
+        self.plot_across_x.update_style('line', visible=False)
+        self.plot_across_x.clear_all_marks()
+        self.plot_across_y.clear_all_marks()
+
     def _create_viewer_callbacks(self, viewer):
         if not self.is_active:
             return
 
         callback = self._viewer_callback(viewer, self._on_viewer_key_event)
         viewer.add_event_callback(callback, events=['keydown'])
 
     def _on_viewer_added(self, msg):
         self._create_viewer_callbacks(self.app.get_viewer_by_id(msg.viewer_id))
 
-    def _get_mark(self, viewer):
-        matches = [mark for mark in viewer.figure.marks if isinstance(mark, MarkersMark)]
-        if len(matches):
-            return matches[0]
-        mark = MarkersMark(viewer)
-        viewer.figure.marks = viewer.figure.marks + [mark]
-        return mark
-
-    @property
-    def marks(self):
-        return {viewer_id: self._get_mark(viewer)
-                for viewer_id, viewer in self.app._viewer_store.items()
-                if hasattr(viewer, 'figure')}
-
-    @property
-    def coords_info(self):
-        return self.app.session.application._tools['g-coords-info']
-
     @observe('is_active')
-    def _on_is_active_changed(self, *args):
-        if self.disabled_msg:
-            return
-
-        # toggle visibility of markers
-        for mark in self.marks.values():
-            mark.visible = self.is_active
-
+    def _is_active_changed(self, msg):
         # subscribe/unsubscribe to keypress events across all viewers
         for viewer in self.app._viewer_store.values():
             if not hasattr(viewer, 'figure'):
                 # table viewer, etc
                 continue
             callback = self._viewer_callback(viewer, self._on_viewer_key_event)
 
             if self.is_active:
                 viewer.add_event_callback(callback, events=['keydown'])
             else:
                 viewer.remove_event_callback(callback)
 
+        # pass along the msg object so that @skip_if_no_updates_since_last_active can be used
+        # to avoid re-drawing if no changes since the last time is_active was set
+        self.vue_draw_plot(msg)
+
     def _on_viewer_key_event(self, viewer, data):
-        if data['event'] == 'keydown' and data['key'] == 'm':
-            row_info = self.coords_info.as_dict()
+        if data['key'] == 'l':
+            image = viewer.active_image_layer.layer
+            x = data['domain']['x']
+            y = data['domain']['y']
+            if x is None or y is None:  # Out of bounds
+                return
+            x, y, _, _ = viewer._get_real_xy(image, x, y)
+            self.selected_x = x
+            self.selected_y = y
+            self.viewer_selected = viewer.reference_id
+            # TODO: remove manual calls to vue_draw_plot and trigger
+            # by changes to selected_x/selected_y as well as viewer_selected
+            self.vue_draw_plot()
+
+    @observe("viewer_selected")
+    @skip_if_no_updates_since_last_active()  # called with msg passed along from _is_active_changed
+    def vue_draw_plot(self, msg={}):
+        """Draw line profile plots for given Data across given X and Y indices (0-indexed)."""
+        if not self.selected_x or not self.selected_y:
+            return
 
-            if 'viewer' in self.table.headers_avail:
-                row_info['viewer'] = viewer.reference if viewer.reference is not None else viewer.reference_id  # noqa
+        viewer = self.viewer.selected_obj
+        i = get_top_layer_index(viewer)
+        data = viewer.state.layers[i].layer
+
+        x = int(round(self.selected_x))
+        y = int(round(self.selected_y))
+
+        nx = data.shape[1]
+        ny = data.shape[0]
+        if x < 0 or y < 0 or x >= nx or y >= ny:
+            self.reset_results()
+            return
+
+        comp = data.get_component(data.main_components[0])
+        if comp.units:
+            y_label = comp.units
+        else:
+            y_label = 'Value'
 
-            for k in self.table.headers_avail:
-                row_info.setdefault(k, self._default_table_values.get(k, ''))
+        xy_limits = viewer._get_zoom_limits(data)
+        x_limits = xy_limits[:, 0]
+        y_limits = xy_limits[:, 1]
+        x_min = max(int(x_limits.min()), 0)
+        x_max = min(int(x_limits.max()), nx)
+        y_min = max(int(y_limits.min()), 0)
+        y_max = min(int(y_limits.max()), ny)
+
+        self.plot_across_x.figure.title = f'X={x}'
+        self.plot_across_x._update_data('line', x=range(comp.data.shape[0]), y=comp.data[:, x],
+                                        reset_lims=False)
+        zoomed_data_x = comp.data[y_min:y_max, x]
+        if zoomed_data_x.size > 0:
+            self.plot_across_x.set_limits(x_min=y_min,
+                                          x_max=y_max,
+                                          y_min=np.nanmin(zoomed_data_x) * 0.95,
+                                          y_max=np.nanmax(zoomed_data_x) * 1.05)
+        self.plot_across_x.update_style('line', line_visible=True,
+                                        markers_visible=False, color='gray', size=10)
+        self.plot_across_x.viewer.axis_x.label = 'Y (pix)'
+        self.plot_across_x.viewer.axis_y.label = y_label
+
+        self.plot_across_y.figure.title = f'Y={y}'
+        self.plot_across_y._update_data('line', x=range(comp.data.shape[1]), y=comp.data[y, :],
+                                        reset_lims=False)
+        zoomed_data_y = comp.data[y, x_min:x_max]
+        if zoomed_data_y.size > 0:
+            self.plot_across_y.set_limits(x_min=x_min,
+                                          x_max=x_max,
+                                          y_min=np.nanmin(zoomed_data_y) * 0.95,
+                                          y_max=np.nanmax(zoomed_data_y) * 1.05)
+        self.plot_across_y.update_style('line', line_visible=True,
+                                        markers_visible=False, color='gray', size=10)
+        self.plot_across_y.viewer.axis_x.label = 'X (pix)'
+        self.plot_across_y.viewer.axis_y.label = y_label
 
-            try:
-                self.table.add_item({k: v for k, v in row_info.items()
-                                     if k in self.table.headers_avail})
-            except ValueError as err:
-                raise ValueError(f'failed to add {row_info} to table: {repr(err)}')
-
-            x, y = row_info['axes_x'], row_info['axes_y']
-            self._get_mark(viewer).append_xy(getattr(x, 'value', x), getattr(y, 'value', y))
-
-    def clear_table(self):
-        """
-        Clear all entries/markers from the current table.
-        """
-        super().clear_table()
-        for mark in self.marks.values():
-            mark.clear()
+        self.plot_available = True
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/markers/tests/test_markers_plugin.py` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/markers/tests/test_markers_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,23 +16,27 @@
             assert_allclose(v, dict2.get(k))
         elif isinstance(v, (tuple, list)):
             assert_allclose(np.asarray(v), np.asarray(dict2.get(k)))
         else:
             assert v == dict2.get(k)
 
 
-def test_markers_cubeviz(cubeviz_helper, spectrum1d_cube):
+def test_markers_cubeviz(tmp_path, cubeviz_helper, spectrum1d_cube):
     cubeviz_helper.load_data(spectrum1d_cube, "test")
     fv = cubeviz_helper.app.get_viewer('flux-viewer')
     sv = cubeviz_helper.app.get_viewer('spectrum-viewer')
 
     label_mouseover = cubeviz_helper.app.session.application._tools['g-coords-info']
 
     mp = cubeviz_helper.plugins['Markers']
     mp.keep_active = True
+    exp = cubeviz_helper.plugins['Export']
+
+    # no marks yet, so table does not yet appear in export plugin
+    assert "Markers: table" not in exp.plugin_table.choices
 
     # test event in flux viewer
     label_mouseover._viewer_mouse_event(fv,
                                         {'event': 'mousemove',
                                          'domain': {'x': 0, 'y': 0}})
 
     assert label_mouseover.as_text() == ('Pixel x=00.0 y=00.0 Value +8.00000e+00 Jy',
@@ -120,14 +124,20 @@
     # markers re-appear when plugin re-opened
     mp._obj.plugin_opened = True
     assert _get_markers_from_viewer(fv).visible is True
     assert _get_markers_from_viewer(sv).visible is True
     assert len(_get_markers_from_viewer(fv).x) == 1
     assert len(_get_markers_from_viewer(sv).x) == 2
 
+    # appears as option in export plugin and exports successfully
+    assert "Markers: table" in exp.plugin_table.choices
+    exp.filename = str(tmp_path / "cubeviz_export.ecsv")
+    exp.plugin_table = "Markers: table"
+    exp.export()
+
     # clearing table clears markers
     mp.clear_table()
     assert mp.export_table() is None
     assert len(_get_markers_from_viewer(fv).x) == 0
     assert len(_get_markers_from_viewer(sv).x) == 0
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.py` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.vue` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.vue`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 <template>
   <j-tray-plugin
-    description='View metadata.'
+    :description="docs_description || 'View metadata.'"
     :link="docs_link || 'https://jdaviz.readthedocs.io/en/'+vdocs+'/'+config+'/plugins.html#metadata-viewer'"
-    :popout_button="popout_button">
+    :popout_button="popout_button"
+    :scroll_to.sync="scroll_to">
 
     <!-- for specviz, we'll allow this to hide for a single entry, but since filters are being
          applied on other configs, we'll always show -->
     <plugin-dataset-select
       :items="dataset_items"
       :selected.sync="dataset_selected"
       :show_if_single_entry="config!='specviz'"
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/metadata_viewer/tests/test_metadata_viewer.py` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/metadata_viewer/tests/test_metadata_viewer.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/model_fitting/fitting_backend.py` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/fitting_backend.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/model_fitting/initializers.py` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/initializers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/model_fitting/model_fitting.py` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/model_fitting.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/model_fitting/model_fitting.vue` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/model_fitting.vue`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 <template>
   <j-tray-plugin
-    description='Fit an analytic model to data or a subset.'
+    :description="docs_description || 'Fit an analytic model to data or a subset.'"
     :link="docs_link || 'https://jdaviz.readthedocs.io/en/'+vdocs+'/'+config+'/plugins.html#model-fitting'"
-    :popout_button="popout_button">
+    :popout_button="popout_button"
+    :scroll_to.sync="scroll_to">
 
     <!-- for mosviz, the entries change on row change, so we want to always show the dropdown
          to make sure that is clear -->
     <plugin-dataset-select
       :items="dataset_items"
       :selected.sync="dataset_selected"
       :show_if_single_entry="config=='mosviz'"
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/model_fitting/tests/test_blackbody.py` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/tests/test_blackbody.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/model_fitting/tests/test_fitting.py` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/tests/test_fitting.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/model_fitting/tests/test_plugin.py` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/model_fitting/tests/test_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -339,18 +339,15 @@
     max_wavelength = spectrum1d_cube_larger.wavelength.max()
 
     # This toolbar selection allows the XRangeROI call below to create a
     # new subset, rather than replacing the previous subset:
     sv.toolbar_active_subset.selected = []
 
     # Now create the new spectral subset:
-    sv.apply_roi(XRangeROI(
-        min=min_wavelength.to(u.m).value,
-        max=max_wavelength.to(u.m).value
-    ))
+    sv.apply_roi(XRangeROI(min=min_wavelength.to_value(u.m), max=max_wavelength.to_value(u.m)))
     assert "Subset 2" in p.spectral_subset.choices
 
     # Select the spectral subset
     p.spectral_subset_selected = "Subset 2"
 
     # Get the data object again (ensures mask == None)
     data = cubeviz_helper.app.data_collection[0].get_object(
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/plot_options/plot_options.py` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/plot_options/plot_options.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,33 +10,60 @@
 from echo import delay_callback
 from traitlets import Any, Dict, Float, Bool, Int, List, Unicode, observe
 
 from glue.core.subset_group import GroupedSubset
 from glue.config import colormaps, stretches
 from glue.viewers.scatter.state import ScatterViewerState
 from glue.viewers.profile.state import ProfileViewerState, ProfileLayerState
-from glue.viewers.image.state import ImageSubsetLayerState
+from glue.viewers.image.state import ImageSubsetLayerState, ImageViewerState
 from glue.viewers.scatter.state import ScatterLayerState as BqplotScatterLayerState
 from glue.viewers.image.composite_array import COLOR_CONVERTER
 from glue_jupyter.bqplot.image.state import BqplotImageLayerState
 from glue_jupyter.common.toolbar_vuetify import read_icon
 
 from jdaviz.core.registries import tray_registry
 from jdaviz.core.template_mixin import (PluginTemplateMixin, ViewerSelect, LayerSelect,
                                         PlotOptionsSyncState, Plot,
                                         skip_if_no_updates_since_last_active, with_spinner)
+from jdaviz.core.events import ChangeRefDataMessage
 from jdaviz.core.user_api import PluginUserApi
 from jdaviz.core.tools import ICON_DIR
 from jdaviz.core.custom_traitlets import IntHandleEmpty
+from jdaviz.utils import is_not_wcs_only
 
-from scipy.interpolate import make_interp_spline
+
+from scipy.interpolate import PchipInterpolator
+from photutils.utils import make_random_cmap
 
 __all__ = ['PlotOptions']
 
 
+def _register_random_cmap(
+    cmap_name,
+    bkg_color=[0, 0, 0],
+    bkg_alpha=1,
+    seed=42,
+    ncolors=10_000
+):
+    """
+    Custom random colormap, useful for rendering image
+    segmentation maps. The default background for
+    `label==0` is *transparent*. If the segmentation map
+    contains more than 10,000 labels, adjust the `ncolors`
+    kwarg to ensure uniqueness.
+    """
+    cmap = make_random_cmap(ncolors=ncolors, seed=seed)
+    cmap.colors[0] = bkg_color + [bkg_alpha]
+    cmap.name = cmap_name
+    colormaps.add(cmap_name, cmap)
+
+
+_register_random_cmap('Random', bkg_alpha=1)
+
+
 class SplineStretch:
     """
     A class to represent spline stretches.
 
     Attributes
     ----------
     k : int
@@ -55,47 +82,58 @@
     Raises
     ------
     ValueError
         If `x` and `y` have different lengths.
     """
 
     def __init__(self):
-        # Cubic Spline (degree 3) for its balance and between accuracy & smoothness.
-        # May revisit when knots become editable.
-        self.k = 3
-        self.bc_type = None
-        self.t = None
-
         # Default x, y values(0-1) range chosen for a typical initial spline shape.
         # Can be modified if required.
-        self.update_knots(
-            x=np.array([0, 0.1, 0.2, 0.7, 1]),
-            y=np.array([0, 0.05, 0.3, 0.9, 1])
-        )
+        self._x = np.array([0, 0.1, 0.2, 0.7, 1])
+        self._y = np.array([0, 0.05, 0.3, 0.9, 1])
+        self.update_knots(self._x, self._y)
+
+    @property
+    def knots(self):
+        return (self._x, self._y)
+
+    @knots.setter
+    def knots(self, value):
+        x, y = value
+        if len(x) != len(y):
+            # Silently return
+            return
+        self.update_knots(x, y)
 
     def __call__(self, values, out=None, clip=False):
         # For our uses, we can ignore `out` and `clip`, but those would need
         # to be implemented before contributing this class upstream.
         return self.spline(values)
 
     def update_knots(self, x, y):
-        if len(x) != len(y):
-            raise ValueError("x and y must be the same length.")
-        self.x = x
-        self.y = y
-        self.spline = make_interp_spline(
-            self.x, self.y, k=self.k, t=self.t, bc_type=self.bc_type
-        )
+        self._x = x
+        self._y = y
+        self.spline = PchipInterpolator(self._x, self._y)
 
 
 # Add the spline stretch to the glue stretch registry if not registered
 if "spline" not in stretches:
     stretches.add("spline", SplineStretch, display="Spline")
 
 
+def _round_step(step):
+    # round the step for a float input
+    if step <= 0:
+        return 1e-6, 6
+    decimals = -int(np.log10(abs(step))) + 1 if step != 0 else 6
+    if decimals < 0:
+        decimals = 0
+    return np.round(step, decimals), decimals
+
+
 @tray_registry('g-plot-options', label="Plot Options")
 class PlotOptions(PluginTemplateMixin):
     """
     The Plot Options Plugin gives access to per-viewer and per-layer options and enables
     setting across multiple viewers/layers simultaneously.
 
     Only the following attributes and methods are available through the
@@ -109,14 +147,16 @@
     * ``layer`` (:class:`~jdaviz.core.template_mixin.LayerSelect`):
     * ``layer_multiselect``
     * :meth:`select_all`
     * ``subset_visible`` (:class:`~jdaviz.core.template_mixin.PlotOptionsSyncState`):
       whether a subset should be visible.
     * ``subset_color`` (:class:`~jdaviz.core.template_mixin.PlotOptionsSyncState`):
       not exposed for Specviz
+    * ``subset_opacity`` (:class:`~jdaviz.core.template_mixin.PlotOptionsSyncState`):
+      not exposed for Specviz
     * ``axes_visible`` (:class:`~jdaviz.core.template_mixin.PlotOptionsSyncState`):
       not exposed for Imviz
     * ``collapse_function`` (:class:`~jdaviz.core.template_mixin.PlotOptionsSyncState`):
       only exposed for Cubeviz
     * ``line_visible`` (:class:`~jdaviz.core.template_mixin.PlotOptionsSyncState`):
       not exposed for Imviz
     * ``line_color`` (:class:`~jdaviz.core.template_mixin.PlotOptionsSyncState`):
@@ -169,17 +209,21 @@
       not exposed for Specviz. This only applies when ``contour_mode`` is "Linear".
     * ``contour_custom_levels`` (:class:`~jdaviz.core.template_mixin.PlotOptionsSyncState`):
       not exposed for Specviz. This only applies when ``contour_mode`` is "Custom".
     """
     template_file = __file__, "plot_options.vue"
     uses_active_status = Bool(True).tag(sync=True)
 
+    # read-only display units
+    display_units = Dict().tag(sync=True)
+
     viewer_multiselect = Bool(False).tag(sync=True)
     viewer_items = List().tag(sync=True)
     viewer_selected = Any().tag(sync=True)  # Any needed for multiselect
+    viewer_limits = Dict().tag(sync=True)
 
     layer_multiselect = Bool(False).tag(sync=True)
     layer_items = List().tag(sync=True)
     layer_selected = Any().tag(sync=True)  # Any needed for multiselect
 
     # profile/line viewer/layer options:
     line_visible_value = Bool().tag(sync=True)
@@ -199,14 +243,40 @@
 
     line_as_steps_value = Bool().tag(sync=True)
     line_as_steps_sync = Dict().tag(sync=True)
 
     uncertainty_visible_value = Int().tag(sync=True)
     uncertainty_visible_sync = Dict().tag(sync=True)
 
+    x_min_value = Float().tag(sync=True)
+    x_min_sync = Dict().tag(sync=True)
+
+    x_max_value = Float().tag(sync=True)
+    x_max_sync = Dict().tag(sync=True)
+
+    y_min_value = Float().tag(sync=True)
+    y_min_sync = Dict().tag(sync=True)
+
+    y_max_value = Float().tag(sync=True)
+    y_max_sync = Dict().tag(sync=True)
+
+    x_bound_step = Float(0.1).tag(sync=True)  # dynamic based on maximum value
+    y_bound_step = Float(0.1).tag(sync=True)  # dynamic based on maximum value
+
+    zoom_center_x_value = Float().tag(sync=True)
+    zoom_center_x_sync = Dict().tag(sync=True)
+
+    zoom_center_y_value = Float().tag(sync=True)
+    zoom_center_y_sync = Dict().tag(sync=True)
+
+    zoom_radius_value = Float().tag(sync=True)
+    zoom_radius_sync = Dict().tag(sync=True)
+
+    zoom_step = Float(1).tag(sync=True)
+
     # scatter/marker options
     marker_visible_value = Bool().tag(sync=True)
     marker_visible_sync = Dict().tag(sync=True)
 
     marker_fill_value = Bool().tag(sync=True)
     marker_fill_sync = Dict().tag(sync=True)
 
@@ -260,27 +330,33 @@
 
     stretch_vmin_value = Float().tag(sync=True)
     stretch_vmin_sync = Dict().tag(sync=True)
 
     stretch_vmax_value = Float().tag(sync=True)
     stretch_vmax_sync = Dict().tag(sync=True)
 
+    stretch_params_value = Dict().tag(sync=True)
+    stretch_params_sync = Dict().tag(sync=True)
+
     stretch_hist_sync = Dict().tag(sync=True)
     stretch_hist_zoom_limits = Bool().tag(sync=True)
     stretch_hist_nbins = IntHandleEmpty(25).tag(sync=True)
     stretch_histogram_widget = Unicode().tag(sync=True)
 
     stretch_curve_visible = Bool(True).tag(sync=True)
 
     subset_visible_value = Bool().tag(sync=True)
     subset_visible_sync = Dict().tag(sync=True)
 
     subset_color_value = Unicode().tag(sync=True)
     subset_color_sync = Dict().tag(sync=True)
 
+    subset_opacity_value = Float().tag(sync=True)
+    subset_opacity_sync = Dict().tag(sync=True)
+
     image_visible_value = Bool().tag(sync=True)
     image_visible_sync = Dict().tag(sync=True)
 
     image_color_mode_value = Unicode().tag(sync=True)
     image_color_mode_sync = Dict().tag(sync=True)
 
     image_color_value = Any().tag(sync=True)
@@ -326,21 +402,24 @@
     icon_checktoradial = Unicode(read_icon(os.path.join(ICON_DIR, 'checktoradial.svg'), 'svg+xml')).tag(sync=True)  # noqa
 
     show_viewer_labels = Bool(True).tag(sync=True)
 
     cmap_samples = Dict().tag(sync=True)
     swatches_palette = List().tag(sync=True)
     apply_RGB_presets_spinner = Bool(False).tag(sync=True)
+    stretch_hist_spinner = Bool(False).tag(sync=True)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.viewer = ViewerSelect(self, 'viewer_items', 'viewer_selected', 'viewer_multiselect')
         self.layer = LayerSelect(self, 'layer_items', 'layer_selected',
                                  'viewer_selected', 'layer_multiselect')
 
+        self.layer.filters += [is_not_wcs_only]
+
         self.swatches_palette = [
             ['#FF0000', '#AA0000', '#550000'],
             ['#FFD300', '#AAAA00', '#555500'],
             ['#4CFF00', '#00AA00', '#005500'],
             ['#00FF8E', '#00AAAA', '#005555'],
             ['#0089FF', '#5200FF', '#000055']
         ]
@@ -359,19 +438,22 @@
 
         def is_image(state):
             return isinstance(state, BqplotImageLayerState)
 
         def not_image(state):
             return not is_image(state)
 
+        def not_image_viewer(state):
+            return not isinstance(state, ImageViewerState)
+
         def not_image_or_spatial_subset(state):
             return not is_image(state) and not is_spatial_subset(state)
 
         def is_spatial_subset(state):
-            return isinstance(state, ImageSubsetLayerState)
+            return isinstance(state, ImageSubsetLayerState) and is_not_wcs_only(state.layer)
 
         def is_not_subset(state):
             return not is_spatial_subset(state)
 
         def line_visible(state):
             # exclude for scatter layers where the marker is shown instead of the line
             return getattr(state, 'line_visible', True)
@@ -397,14 +479,34 @@
                                                  'line_opacity_value', 'line_opacity_sync',
                                                  state_filter=supports_line)
         self.line_as_steps = PlotOptionsSyncState(self, self.viewer, self.layer, 'as_steps',
                                                   'line_as_steps_value', 'line_as_steps_sync')
         self.uncertainty_visible = PlotOptionsSyncState(self, self.viewer, self.layer, 'show_uncertainty',  # noqa
                                                         'uncertainty_visible_value', 'uncertainty_visible_sync')  # noqa
 
+        # Viewer bounds
+        self.x_min = PlotOptionsSyncState(self, self.viewer, self.layer, 'x_min',
+                                          'x_min_value', 'x_min_sync',
+                                          state_filter=not_image_viewer)
+        self.x_max = PlotOptionsSyncState(self, self.viewer, self.layer, 'x_max',
+                                          'x_max_value', 'x_max_sync',
+                                          state_filter=not_image_viewer)
+        self.y_min = PlotOptionsSyncState(self, self.viewer, self.layer, 'y_min',
+                                          'y_min_value', 'y_min_sync',
+                                          state_filter=not_image_viewer)
+        self.y_max = PlotOptionsSyncState(self, self.viewer, self.layer, 'y_max',
+                                          'y_max_value', 'y_max_sync',
+                                          state_filter=not_image_viewer)
+        self.zoom_center_x = PlotOptionsSyncState(self, self.viewer, self.layer, 'zoom_center_x',
+                                                  'zoom_center_x_value', 'zoom_center_x_sync')
+        self.zoom_center_y = PlotOptionsSyncState(self, self.viewer, self.layer, 'zoom_center_y',
+                                                  'zoom_center_y_value', 'zoom_center_y_sync')
+        self.zoom_radius = PlotOptionsSyncState(self, self.viewer, self.layer, 'zoom_radius',
+                                                'zoom_radius_value', 'zoom_radius_sync')
+
         # Scatter/marker options:
         # NOTE: marker_visible hides the entire layer (including the line)
         self.marker_visible = PlotOptionsSyncState(self, self.viewer, self.layer, 'visible',
                                                    'marker_visible_value', 'marker_visible_sync',
                                                    state_filter=is_scatter)
         self.marker_fill = PlotOptionsSyncState(self, self.viewer, self.layer, 'fill',
                                                 'marker_fill_value', 'marker_fill_sync',
@@ -463,16 +565,19 @@
                                                    state_filter=is_image)
         self.stretch_vmin = PlotOptionsSyncState(self, self.viewer, self.layer, 'v_min',
                                                  'stretch_vmin_value', 'stretch_vmin_sync',
                                                  state_filter=is_image)
         self.stretch_vmax = PlotOptionsSyncState(self, self.viewer, self.layer, 'v_max',
                                                  'stretch_vmax_value', 'stretch_vmax_sync',
                                                  state_filter=is_image)
+        self.stretch_params = PlotOptionsSyncState(self, self.viewer, self.layer, 'stretch_parameters',  # noqa
+                                                   'stretch_params_value', 'stretch_params_sync',
+                                                   state_filter=is_image)
 
-        self.stretch_histogram = Plot(self, viewer_type='histogram')
+        self.stretch_histogram = Plot(self, name='stretch_hist', viewer_type='histogram')
         # Add the stretch bounds tool to the default Plot viewer.
         self.stretch_histogram.tools_nested.append(["jdaviz:stretch_bounds"])
         self.stretch_histogram._initialize_toolbar(["jdaviz:stretch_bounds"])
 
         self.stretch_histogram._add_data('histogram', x=[0, 1])
 
         self.stretch_histogram.add_line('vmin', x=[0, 0], y=[0, 1], ynorm=True, color='#c75d2c')
@@ -484,15 +589,15 @@
             color="#007BA1",  # "inactive" blue
             opacities=[0.5],
         )
         self.stretch_histogram.add_scatter(
             label='stretch_knots',
             x=[], y=[],
             ynorm='vmin',
-            color="#007BA1",  # "inactive" blue
+            color="#c75d2c",  # "active" orange (tool enabled by default)
         )
         self.stretch_histogram.add_scatter('colorbar', x=[], y=[], ynorm='vmin', marker='square', stroke_width=33)  # noqa: E501
         self.stretch_histogram.viewer.state.update_bins_on_reset_limits = False
         self.stretch_histogram.viewer.state.x_limits_percentile = 95
         with self.stretch_histogram.figure.hold_sync():
             self.stretch_histogram.figure.axes[0].label = 'pixel value'
             self.stretch_histogram.figure.axes[0].num_ticks = 3
@@ -503,14 +608,17 @@
 
         self.subset_visible = PlotOptionsSyncState(self, self.viewer, self.layer, 'visible',
                                                    'subset_visible_value', 'subset_visible_sync',
                                                    state_filter=is_spatial_subset)
         self.subset_color = PlotOptionsSyncState(self, self.viewer, self.layer, 'color',
                                                  'subset_color_value', 'subset_color_sync',
                                                  state_filter=is_spatial_subset)
+        self.subset_opacity = PlotOptionsSyncState(self, self.viewer, self.layer, 'alpha',
+                                                   'subset_opacity_value', 'subset_opacity_sync',
+                                                   state_filter=is_spatial_subset)
         self.image_visible = PlotOptionsSyncState(self, self.viewer, self.layer, 'bitmap_visible',
                                                   'image_visible_value', 'image_visible_sync',
                                                   state_filter=is_image)
         self.image_color_mode = PlotOptionsSyncState(self, self.viewer, self.layer, 'color_mode',  # noqa
                                                      'image_color_mode_value', 'image_color_mode_sync')  # noqa
         self.image_color = PlotOptionsSyncState(self, self.viewer, self.layer, 'color',
                                                 'image_color_value', 'image_color_sync',
@@ -545,38 +653,48 @@
                                                           spinner='contour_spinner')
 
         # Axes options:
         # axes_visible hidden for imviz in plot_options.vue
         self.axes_visible = PlotOptionsSyncState(self, self.viewer, self.layer, 'show_axes',
                                                  'axes_visible_value', 'axes_visible_sync',
                                                  state_filter=not_profile)
-        # zoom limits
-        # display_units
 
         self.show_viewer_labels = self.app.state.settings['viewer_labels']
         self.app.state.add_callback('settings', self._on_app_settings_changed)
 
+        sv = self.spectrum_viewer
+        if sv is not None:
+            sv.state.add_callback('x_display_unit',
+                                  self._on_global_display_unit_changed)
+            sv.state.add_callback('y_display_unit',
+                                  self._on_global_display_unit_changed)
+
+        self.hub.subscribe(self, ChangeRefDataMessage,
+                           handler=self._on_refdata_change)
+
         # give UI access to sampled version of the available colormap choices
         def hex_for_cmap(cmap):
             N = 50
             cm_sampled = cmap.resampled(N)
             return [matplotlib.colors.to_hex(cm_sampled(i)) for i in range(N)]
         self.cmap_samples = {cmap[1].name: hex_for_cmap(cmap[1]) for cmap in colormaps.members}
 
     @property
     def user_api(self):
         expose = ['multiselect', 'viewer', 'viewer_multiselect', 'layer', 'layer_multiselect',
                   'select_all', 'subset_visible']
         if self.config == "cubeviz":
             expose += ['collapse_function', 'uncertainty_visible']
         if self.config != "imviz":
-            expose += ['axes_visible', 'line_visible', 'line_color', 'line_width', 'line_opacity',
+            expose += ['x_min', 'x_max', 'y_min', 'y_max',
+                       'axes_visible', 'line_visible', 'line_color', 'line_width', 'line_opacity',
                        'line_as_steps', 'uncertainty_visible']
         if self.config != "specviz":
-            expose += ['subset_color',
+            expose += ['zoom_center_x', 'zoom_center_y', 'zoom_radius',
+                       'subset_color', 'subset_opacity',
                        'stretch_function', 'stretch_preset', 'stretch_vmin', 'stretch_vmax',
                        'stretch_hist_zoom_limits', 'stretch_hist_nbins',
                        'image_visible', 'image_color_mode',
                        'image_color', 'image_colormap', 'image_opacity',
                        'image_contrast', 'image_bias',
                        'contour_visible', 'contour_mode',
                        'contour_min', 'contour_max', 'contour_nlevels', 'contour_custom_levels',
@@ -617,20 +735,40 @@
         if viewers:
             self.viewer_multiselect = True
             self.viewer.select_all()
         if layers:
             self.layer_multiselect = True
             self.layer.select_all()
 
+    def _on_global_display_unit_changed(self, *args):
+        sv = self.spectrum_viewer
+        self.display_units['spectral'] = sv.state.x_display_unit
+        self.display_units['flux'] = sv.state.y_display_unit
+        self.send_state('display_units')
+
+    def _on_refdata_change(self, *args):
+        if self.app._link_type.lower() == 'wcs':
+            self.display_units['image'] = 'deg'
+        else:
+            self.display_units['image'] = 'pix'
+        self.send_state('display_units')
+        self._update_viewer_zoom_steps()
+
     def vue_unmix_state(self, names):
         if isinstance(names, str):
             names = [names]
         for name in names:
             sync_state = getattr(self, name)
             sync_state.unmix_state()
+        if 'stretch_params' in names:
+            # there is no way to call send_state to force the update to the layers,
+            # so we'll force an update by clearing first
+            stretch_params = dict(self.stretch_params_value)
+            self.stretch_params_value = {}
+            self.stretch_params_value = stretch_params
 
     def vue_set_value(self, data):
         attr_name = data.get('name')
         value = data.get('value')
         setattr(self, attr_name, value)
 
     @with_spinner('apply_RGB_presets_spinner')
@@ -664,16 +802,18 @@
         default_opacity = 1
         if n_visible > 2:
             default_opacity = 1 / math.log2(n_visible)
 
         # Sample along a colormap if we have too many layers
         if n_visible > len(preset_colors):
             cmap = matplotlib.colormaps['gist_rainbow'].resampled(n_visible)
+            # Have to reverse the order of the cmap to make physical sense with
+            # assumed wavelength order of layers.
             preset_colors = [matplotlib.colors.to_hex(cmap(i), keep_alpha=True) for
-                             i in range(n_visible)]
+                             i in range(n_visible - 1, -1, -1)]
         elif n_visible >= 2 and n_visible < len(preset_colors):
             preset_colors = [preset_colors[i] for i in preset_inds[n_visible]]
 
         for i in range(n_visible):
             self.layer_selected = visible_layers[i]
             self.image_opacity.unmix_state(default_opacity)
             self.image_color.unmix_state(preset_colors[i])
@@ -681,28 +821,82 @@
             self.stretch_preset.unmix_state(99)
 
         self.layer_selected = initial_layer
 
     def vue_apply_RGB_presets(self, data):
         self.apply_RGB_presets()
 
-    @observe('stretch_function_sync', 'stretch_vmin_sync', 'stretch_vmax_sync',
+    @observe('viewer_selected',
+             'x_min_value', 'x_max_value',
+             'y_min_value', 'y_max_value')
+    def _update_viewer_bound_steps(self, msg={}):
+        if not hasattr(self, 'viewer'):  # pragma: no cover
+            # plugin hasn't been fully initialized yet
+            return
+
+        if not self.viewer.selected or not self.x_min_sync['in_subscribed_states']:
+            # nothing selected yet
+            return
+
+        for ax in ('x', 'y'):
+            ax_min = getattr(self, f'{ax}_min_value')
+            ax_max = getattr(self, f'{ax}_max_value')
+            bound_step, decimals = _round_step((ax_max - ax_min) / 100.)
+            decimals = -int(np.log10(abs(bound_step))) + 1 if bound_step != 0 else 6
+            setattr(self, f'{ax}_bound_step', bound_step)
+            setattr(self, f'{ax}_min_value', np.round(ax_min, decimals=decimals))
+            setattr(self, f'{ax}_max_value', np.round(ax_max, decimals=decimals))
+
+    @observe('viewer_selected',
+             'zoom_center_x_value', 'zoom_center_y_value',
+             'zoom_radius_value')
+    def _update_viewer_zoom_steps(self, msg={}):
+        if not hasattr(self, 'viewer'):  # pragma: no cover
+            # plugin hasn't been fully initialized yet
+            return
+
+        if not self.viewer.selected or not self.zoom_radius_sync['in_subscribed_states']:
+            # nothing selected yet
+            return
+
+        # in the case of multiple viewers, calculate based on the first
+        # alternatively, we could find the most extreme by looping over all selected viewers
+        viewers = self.viewer.selected_obj if self.viewer_multiselect else [self.viewer.selected_obj]  # noqa
+        for viewer in viewers:
+            if hasattr(viewer.state, '_get_reset_limits'):
+                break
+        else:
+            # no image viewer
+            return
+        x_min, x_max, y_min, y_max = viewer.state._get_reset_limits(return_as_world=True)
+        self.zoom_step, _ = _round_step(max(x_max-x_min, y_max-y_min) / 100.)
+
+    def vue_reset_viewer_bounds(self, _):
+        # This button is currently only exposed if only the spectrum viewer is selected
+        viewers = [self.viewer.selected_obj] if not self.viewer_multiselect else self.viewer.selected_obj # noqa
+        for viewer in viewers:
+            viewer.toolbar.tools['jdaviz:homezoom'].activate()
+
+    @observe('stretch_function_sync', 'stretch_params_sync',
+             'stretch_vmin_sync', 'stretch_vmax_sync',
              'image_color_mode_sync', 'image_color_sync', 'image_colormap_sync')
     def _update_stretch_hist_sync(self, msg={}):
         # the histogram should show as mixed if ANY of the input parameters are mixed
         # these should match in the @observe above, all_syncs here, as well as the strings
         # passed to unmix_state in the <glue-state-sync-wrapper> in plot_options.vue
-        all_syncs = [self.stretch_function_sync, self.stretch_vmin_sync, self.stretch_vmax_sync,
+        all_syncs = [self.stretch_function_sync, self.stretch_params_sync,
+                     self.stretch_vmin_sync, self.stretch_vmax_sync,
                      self.image_color_mode_sync, self.image_color_sync, self.image_colormap_sync]
         self.stretch_hist_sync = {'in_subscribed_states': bool(np.any([sync.get('in_subscribed_states', False) for sync in all_syncs])),  # noqa
                                   'mixed': bool(np.any([sync.get('mixed', False) for sync in all_syncs]))}  # noqa
 
     @observe('is_active', 'layer_selected', 'viewer_selected',
              'stretch_hist_zoom_limits')
     @skip_if_no_updates_since_last_active()
+    @with_spinner('stretch_hist_spinner')
     def _update_stretch_histogram(self, msg={}):
         if not hasattr(self, 'viewer'):  # pragma: no cover
             # plugin hasn't been fully initialized yet
             return
 
         if not isinstance(msg, dict):  # pragma: no cover
             # then this is from the limits callbacks
@@ -753,37 +947,42 @@
         if not len(self.layer.selected_obj):
             # skip further updates if no data are available:
             return
         if isinstance(self.layer.selected_obj[0], list):
             if not len(self.layer.selected_obj[0]):
                 return
             # multiselect case (but we won't check multiselect since the selection can lag behind)
-            data = self.layer.selected_obj[0][0].layer
+            layer = self.layer.selected_obj[0][0]
         else:
-            data = self.layer.selected_obj[0].layer
+            layer = self.layer.selected_obj[0]
+        data = layer.layer
 
         if isinstance(data, GroupedSubset):
             # don't update histogram for subsets:
             return
 
-        comp = data.get_component(data.main_components[0])
+        comp = data.get_component(layer.state.attribute)
 
         # TODO: further optimization could be done by caching sub_data
         if self.stretch_hist_zoom_limits and (not self.layer_multiselect or len(self.layer_selected) == 1):  # noqa
             if hasattr(viewer, '_get_zoom_limits'):
                 # Viewer limits. This takes account of Imviz linking.
                 xy_limits = viewer._get_zoom_limits(data).astype(int)
                 x_limits = xy_limits[:, 0]
                 y_limits = xy_limits[:, 1]
                 x_min = max(x_limits.min(), 0)
                 x_max = x_limits.max()
                 y_min = max(y_limits.min(), 0)
                 y_max = y_limits.max()
-
                 arr = comp.data[y_min:y_max, x_min:x_max]
+                if self.config == "imviz":
+                    # Downsample input data to about 400px (as per compass.vue) for performance.
+                    xstep = max(1, round(arr.shape[1] / 400))
+                    ystep = max(1, round(arr.shape[0] / 400))
+                    arr = arr[::ystep, ::xstep]
                 sub_data = arr.ravel()
 
             else:
                 # spectrum-2d-viewer, for example.  We'll assume the viewer
                 # limits correspond to the fixed data components from glue
                 # and filter directly.
                 x_data = data.get_component(data.components[1]).data
@@ -796,16 +995,22 @@
                                 (x_data <= x_max) &
                                 (y_data >= viewer.state.y_min) &
                                 (y_data <= viewer.state.y_max))
 
                 sub_data = comp.data[inds].ravel()
 
         else:
-            # include all data, regardless of zoom limits
-            arr = comp.data
+            if self.config == "imviz":
+                # Downsample input data to about 400px (as per compass.vue) for performance.
+                xstep = max(1, round(data.shape[1] / 400))
+                ystep = max(1, round(data.shape[0] / 400))
+                arr = comp[::ystep, ::xstep]
+            else:
+                # include all data, regardless of zoom limits
+                arr = comp.data
             sub_data = arr.ravel()
 
         # filter out nans (or else bqplot will fail)
         if np.any(np.isnan(sub_data)):
             sub_data = sub_data[~np.isnan(sub_data)]
 
         self.stretch_histogram._update_data('histogram', x=sub_data)
@@ -814,15 +1019,15 @@
             interval = PercentileInterval(95)
             hist_lims = interval.get_limits(sub_data)
             # set the stepsize for vmin/vmax to be approximately 1% of the range of the
             # histogram (within the percentile interval), rounded to 1-2 significant digits
             # to avoid random step sizes.  This logic is somewhat arbitrary and can be safely
             # modified or eventually exposed to the user if that would be useful.
             stretch_vstep = (hist_lims[1] - hist_lims[0]) / 100.
-            self.stretch_vstep = np.round(stretch_vstep, decimals=-int(np.log10(stretch_vstep))+1)  # noqa
+            self.stretch_vstep = _round_step(stretch_vstep)[0]
 
             with delay_callback(self.stretch_histogram.viewer.state, 'hist_x_min', 'hist_x_max'):
                 self.stretch_histogram.viewer.state.hist_x_min = hist_lims[0]
                 self.stretch_histogram.viewer.state.hist_x_max = hist_lims[1]
 
         self.stretch_histogram.figure.title = f"{len(sub_data)} pixels"
 
@@ -832,14 +1037,15 @@
         self._update_stretch_curve(msg)
 
     @observe('image_color_mode_value', 'image_color_value', 'image_colormap_value',
              'image_contrast_value', 'image_bias_value',
              'stretch_hist_nbins',
              'stretch_curve_visible',
              'stretch_function_value', 'stretch_vmin_value', 'stretch_vmax_value',
+             'stretch_params_value', 'stretch_preset_value',
              'layer_multiselect'
              )
     @skip_if_no_updates_since_last_active()
     def _update_stretch_curve(self, msg=None):
         if not self._viewer_is_image_viewer() or not hasattr(self, 'stretch_histogram'):
             # don't update histogram if selected viewer is not an image viewer,
             # or the stretch histogram hasn't been initialized:
@@ -863,15 +1069,14 @@
             return
 
         # create the new/updated stretch curve following the colormapping
         # procedure in glue's CompositeArray:
         interval = ManualInterval(self.stretch_vmin_value, self.stretch_vmax_value)
         contrast_bias = ContrastBiasStretch(self.image_contrast_value, self.image_bias_value)
         stretch = layer.state.stretch_object
-
         layer_cmap = layer.state.cmap
 
         # show the colorbar
         color_mode = self.image_color_mode_value
 
         # NOTE: Index 0 in marks is assumed to be the bin centers.
         x = self.stretch_histogram.figure.marks[0].x
@@ -907,32 +1112,29 @@
         colorbar_mark.y = y
         colorbar_mark.colors = ipycolors
 
         # show "knot" locations if the stretch_function is a spline
         if isinstance(stretch, SplineStretch) and self.stretch_curve_visible:
             knot_mark = self.stretch_histogram.marks['stretch_knots']
             knot_mark.x = (self.stretch_vmin_value +
-                           stretch.x * (self.stretch_vmax_value - self.stretch_vmin_value))
+                           np.asarray(stretch._x) * (self.stretch_vmax_value - self.stretch_vmin_value))  # noqa
             # scale to 0.9 so always falls below colorbar (same as for stretch_curve)
-            # (may need to revisit this when supporting dragging)
-            knot_mark.y = 0.9 * stretch.y
+            knot_mark.y = 0.9 * np.asarray(stretch._y)
         else:
             self.stretch_histogram.clear_marks('stretch_knots')
 
         if self.stretch_curve_visible:
             # create a photoshop style "curve" for the stretch function
             curve_x = np.linspace(self.stretch_vmin_value, self.stretch_vmax_value, 50)
             curve_y = interval(curve_x)
             curve_y = contrast_bias(curve_y)
             curve_y = stretch(curve_y)
 
             curve_mark = self.stretch_histogram.marks['stretch_curve']
             curve_mark.x = curve_x
-            # scale to 0.9 so always falls below colorbar (same as for stretch_knots)
-            # (may need to revisit this when supporting dragging)
             curve_mark.y = 0.9 * curve_y
         else:
             self.stretch_histogram.clear_marks('stretch_curve')
 
         self.stretch_histogram._refresh_marks()
 
     @observe('stretch_vmin_value')
@@ -971,7 +1173,23 @@
                                        MosvizImageView, MosvizProfile2DView))
 
         viewers = self.viewer.selected_obj
         if not isinstance(viewers, list):
             viewers = [viewers]
 
         return np.all([_is_image_viewer(viewer) for viewer in viewers])
+
+    def image_segmentation_map_presets(self, *args, **kwargs):
+        # if 'Random' colormap is used for visualizing image segmentation,
+        # ensure the stretch limits are the min and max, the stretch function
+        # is linear, the contrast is 1.0, and the bias is 0.5. This ensures
+        # that all label colors are unique:
+        if self.image_colormap_value != 'Random':
+            return
+
+        self.stretch_preset.value = 100
+        self.stretch_function.value = 'linear'
+        self.image_contrast_value = 1
+        self.image_bias_value = 0.5
+
+    def vue_image_segmentation_map_presets(self, *args, **kwargs):
+        self.image_segmentation_map_presets(*args, **kwargs)
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/plot_options/plot_options.vue` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/plot_options/plot_options.vue`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 <template>
   <j-tray-plugin
-    description='Viewer and data/layer options.'
+    :description="docs_description || 'Viewer and data/layer options.'"
     :link="docs_link || 'https://jdaviz.readthedocs.io/en/'+vdocs+'/'+config+'/plugins.html#plot-options'"
     :uses_active_status="uses_active_status"
     @plugin-ping="plugin_ping($event)"
-    :popout_button="popout_button">
+    :popout_button="popout_button"
+    :scroll_to.sync="scroll_to">
 
     <v-row>
       <v-expansion-panels popout>
         <v-expansion-panel>
           <v-expansion-panel-header v-slot="{ open }">
             <span style="padding: 6px">Settings</span>
           </v-expansion-panel-header>
@@ -35,14 +36,104 @@
       :icon_checktoradial="icon_checktoradial"
       :icon_radialtocheck="icon_radialtocheck"
       :label="viewer_multiselect ? 'Viewers' : 'Viewer'"
       :show_if_single_entry="viewer_multiselect"
       :hint="viewer_multiselect ? 'Select viewers to set options simultaneously' : 'Select the viewer to set options.'"
     />
 
+    <v-row v-if="viewer_selected.length > 0">
+      <v-expansion-panels accordion>
+        <v-expansion-panel>
+          <v-expansion-panel-header v-slot="{ open }">
+            <span style="padding: 6px">Viewer bounds</span>
+          </v-expansion-panel-header>
+          <v-expansion-panel-content class="plugin-expansion-panel-content">
+            <glue-state-sync-wrapper :sync="x_min_sync" :multiselect="viewer_multiselect" @unmix-state="unmix_state('x_min')">
+              <glue-float-field
+                ref="x_min"
+                label="X Min"
+                :value.sync="x_min_value"
+                type="number"
+                :step="x_bound_step"
+                :suffix="display_units['spectral']"
+              />
+            </glue-state-sync-wrapper>
+            <glue-state-sync-wrapper :sync="x_max_sync" :multiselect="viewer_multiselect" @unmix-state="unmix_state('x_max')">
+              <glue-float-field
+                ref="x_max"
+                label="X Max"
+                :value.sync="x_max_value"
+                type="number"
+                :step="x_bound_step"
+                :suffix="display_units['spectral']"
+              />
+            </glue-state-sync-wrapper>
+            <glue-state-sync-wrapper :sync="y_min_sync" :multiselect="viewer_multiselect" @unmix-state="unmix_state('y_min')">
+              <glue-float-field
+                ref="y_min"
+                label="Y Min"
+                :value.sync="y_min_value"
+                type="number"
+                :step="y_bound_step"
+                :suffix="display_units['flux']"
+              />
+            </glue-state-sync-wrapper>
+            <glue-state-sync-wrapper :sync="y_max_sync" :multiselect="viewer_multiselect" @unmix-state="unmix_state('y_max')">
+              <glue-float-field
+                ref="y_max"
+                label="Y Max"
+                :value.sync="y_max_value"
+                type="number"
+                :step="y_bound_step"
+                :suffix="display_units['flux']"
+              />
+            </glue-state-sync-wrapper>
+            <glue-state-sync-wrapper :sync="zoom_center_x_sync" :multiselect="viewer_multiselect" @unmix-state="unmix_state('zoom_center_x')">
+              <glue-float-field
+                ref="zoom_center_x"
+                label="X Center"
+                :value.sync="zoom_center_x_value"
+                type="number"
+                :step="zoom_step"
+                :suffix="display_units['image'] || 'pix'"
+              />
+            </glue-state-sync-wrapper>
+            <glue-state-sync-wrapper :sync="zoom_center_y_sync" :multiselect="viewer_multiselect" @unmix-state="unmix_state('zoom_center_y')">
+              <glue-float-field
+                ref="zoom_center_y"
+                label="Y Center"
+                :value.sync="zoom_center_y_value"
+                type="number"
+                :step="zoom_step"
+                :suffix="display_units['image'] || 'pix'"
+              />
+            </glue-state-sync-wrapper>
+            <glue-state-sync-wrapper :sync="zoom_radius_sync" :multiselect="viewer_multiselect" @unmix-state="unmix_state('zoom_radius')">
+              <glue-float-field
+                ref="zoom_radius"
+                label="Zoom-radius"
+                :value.sync="zoom_radius_value"
+                type="number"
+                :step="zoom_step"
+                :suffix="display_units['image'] || 'pix'"
+              />
+            </glue-state-sync-wrapper>
+            <v-row justify="end">
+              <plugin-action-button
+                :results_isolated_to_plugin="false"
+                @click="reset_viewer_bounds"
+              >
+                Reset viewer bounds
+              </plugin-action-button>
+            </v-row>
+          </v-expansion-panel-content>
+        </v-expansion-panel>
+      </v-expansion-panels>
+    </v-row>
+
     <div v-if="image_color_mode_sync.in_subscribed_states">
       <glue-state-sync-wrapper :sync="image_color_mode_sync" :multiselect="viewer_multiselect" @unmix-state="unmix_state('image_color_mode')">
         <v-select
           attach
           :menu-props="{ left: true }"
           :items="image_color_mode_sync.choices"
           v-model="image_color_mode_value"
@@ -65,18 +156,18 @@
             Assign RGB Presets
           </plugin-action-button>
         </j-tooltip>
       </v-row>
     </div>
 
     <!-- GENERAL:AXES -->
-    <glue-state-sync-wrapper v-if="axes_visible_sync.in_subscribed_states && config !== 'imviz'" :sync="axes_visible_sync" :multiselect="viewer_multiselect" @unmix-state="unmix_state('axes_visible')">
+    <glue-state-sync-wrapper v-if="axes_visible_sync.in_subscribed_states && viewer_selected.length > 0 && config !== 'imviz'" :sync="axes_visible_sync" :multiselect="viewer_multiselect" @unmix-state="unmix_state('axes_visible')">
       <v-switch
         v-model="axes_visible_value"
-        label="Show Axes"
+        label="Show axes"
         />
     </glue-state-sync-wrapper>
 
     <glue-state-sync-wrapper v-if="uncertainty_visible_sync.in_subscribed_states" :sync="uncertainty_visible_sync" :multiselect="viewer_multiselect" @unmix-state="unmix_state('uncertainty_visible')">
       <v-switch
         v-model="uncertainty_visible_value"
         label="Plot uncertainties"
@@ -143,14 +234,21 @@
                 <v-color-picker :value="subset_color_value"
                                 @update:color="throttledSetValue('subset_color_value', $event.hexa)"></v-color-picker>
             </div>
           </v-menu>
         </div>
       </glue-state-sync-wrapper>
 
+      <glue-state-sync-wrapper :sync="subset_opacity_sync" :multiselect="layer_multiselect" @unmix-state="unmix_state('subset_opacity')">
+        <div>
+          <v-subheader class="pl-0 slider-label" style="height: 12px">Subset Opacity</v-subheader>
+          <glue-throttled-slider wait="300" max="1" step="0.01" :value.sync="subset_opacity_value" hide-details class="no-hint" />
+        </div>
+      </glue-state-sync-wrapper>
+
 
       <!-- PROFILE/LINE -->
       <j-plugin-section-header v-if="(line_visible_sync.in_subscribed_states && ((!marker_visible_sync.in_subscribed_states && line_visible_value) || (marker_visible_sync.in_subscribed_states && marker_visible_value))) || collapse_func_sync.in_subscribed_states">Line</j-plugin-section-header>
       <glue-state-sync-wrapper v-if="marker_visible_sync.in_subscribed_states && marker_visible_value" :sync="line_visible_sync" :multiselect="layer_multiselect" @unmix-state="unmix_state('line_visible')">
         <span>
           <v-btn icon @click.stop="line_visible_value = !line_visible_value">
             <v-icon>mdi-eye{{ line_visible_value ? '' : '-off' }}</v-icon>
@@ -371,14 +469,32 @@
             attach
             :menu-props="{ left: true }"
             :items="image_colormap_sync.choices"
             v-model="image_colormap_value"
             label="Colormap"
             dense
           ></v-select>
+              <v-alert v-if="image_colormap_value == 'Random' && (
+                  stretch_function_value !== 'linear' || stretch_preset_value !== 100 ||
+                  image_bias_value !== 0.5 || image_contrast_value !== 1.0
+                  )" type='warning' style="margin-left: -12px; margin-right: -12px">
+                For image segmentation maps, "Random" gives unique colors
+                only when the stretch percentile is min/max, stretch function
+                is linear, contrast is 1.0, and bias is 0.5. Click below
+                to choose these settings.
+                <v-row justify='end'>
+                <plugin-action-button
+                  :results_isolated_to_plugin="true"
+                  @click="image_segmentation_map_presets"
+                >
+                  Image segmentation map
+                </plugin-action-button>
+                </v-row>
+              </v-alert>
+
         </glue-state-sync-wrapper>
         <glue-state-sync-wrapper v-if="image_color_mode_value !== 'Colormaps' || image_color_mode_sync['mixed']" :sync="image_color_sync" :multiselect="layer_multiselect" @unmix-state="unmix_state('image_color')">
           <div>
             <v-subheader class="pl-0 slider-label" style="height: 12px; margin-bottom: 4px">Image Color</v-subheader>
             <v-menu>
               <template v-slot:activator="{ on }">
                   <span class="color-menu"
@@ -461,22 +577,41 @@
           v-model.number="stretch_vmax_value"
           type="number"
           :step="stretch_vstep"
         ></v-text-field>
       </glue-state-sync-wrapper>
 
       <div v-if="stretch_function_sync.in_subscribed_states && (!layer_multiselect || layer_selected.length <= 1)">
-        <glue-state-sync-wrapper 
-            :sync="stretch_hist_sync"
-            :multiselect="layer_multiselect" 
-            @unmix-state="unmix_state(['stretch_function', 'stretch_vmin', 'stretch_vmax',
-                                       'image_color_mode', 'image_color', 'image_colormap'])"
-        >
-          <jupyter-widget :widget="stretch_histogram_widget"/>
-        </glue-state-sync-wrapper>
+        <div style="display: grid"> <!-- overlay container -->
+          <div style="grid-area: 1/1">
+            <glue-state-sync-wrapper
+                :sync="stretch_hist_sync"
+                :multiselect="layer_multiselect"
+                @unmix-state="unmix_state(['stretch_function', 'stretch_params',
+                                           'stretch_vmin', 'stretch_vmax',
+                                           'image_color_mode', 'image_color', 'image_colormap'])"
+            >
+              <jupyter-widget :widget="stretch_histogram_widget"/>
+            </glue-state-sync-wrapper>
+          </div>
+          <div v-if="stretch_hist_spinner"
+               class="text-center"
+               style="grid-area: 1/1;
+                      z-index:2;
+                      margin-left: -24px;
+                      margin-right: -24px;
+                      padding-top: 240px;
+                      background-color: rgb(0 0 0 / 20%)">
+            <v-progress-circular
+              indeterminate
+              color="spinner"
+              size="50"
+              width="6"
+            ></v-progress-circular>
+          </div>
 
         <v-row>
           <v-expansion-panels accordion>
             <v-expansion-panel>
               <v-expansion-panel-header v-slot="{ open }">
                 <span style="padding: 6px">More Stretch Options</span>
               </v-expansion-panel-header>
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/plot_options/tests/test_plot_options.py` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/plot_options/tests/test_plot_options.py`

 * *Files 5% similar despite different names*

```diff
@@ -173,17 +173,17 @@
 
     po.viewer = 'flux-viewer'
     po.layer.select_all()
 
     # check a plot option with and without choices
     assert hasattr(po.stretch_preset, 'choices')
     assert len(po.stretch_preset.choices) > 1
-    assert "choices" in po.stretch_preset.__repr__()
+    assert "choices" in po.stretch_preset._obj.__repr__()
     assert not hasattr(po.image_contrast, 'choices')
-    assert "choices" not in po.image_contrast.__repr__()
+    assert "choices" not in po.image_contrast._obj.__repr__()
 
     # try setting with both label and value
     po.stretch_preset = 90
     po.stretch_preset = 'Min/Max'
 
     # try eq on both text and value
     assert po.image_colormap == 'gray'
@@ -284,33 +284,37 @@
     po.layer = "array_5"
     po.image_visible = False
     po.layer = "array_3"
 
     po.apply_RGB_presets()
 
     assert po.layer.selected == "array_3"
+    assert po.stretch_function.value == "arcsinh"
+    po.layer = "array_5"
+    # Make sure this one didn't change
+    assert po.stretch_function.value == "linear"
+
+    # Turn layer 5 back on
+    po.image_visible = True
+    po.apply_RGB_presets()
 
-    colorbar_colors = matplotlib.colormaps['gist_rainbow'].resampled(7)
+    colorbar_colors = matplotlib.colormaps['gist_rainbow'].resampled(8)
     color_ind = 0
 
     def _rgb_to_hex(rgb):
         rgb = [int(x * 255) for x in rgb]
         return f"#{rgb[0]:02x}{rgb[1]:02x}{rgb[2]:02x}{rgb[3]:02x}"
 
     for i in range(8):
         po.layer = f"array_{i}"
-        if i == 5:
-            # Make sure this one didn't change
-            assert po.stretch_function.value == "linear"
-        else:
-            assert po.stretch_function.value == "arcsinh"
-            assert po.stretch_preset.value == 99
-            assert po.image_color.value == matplotlib.colors.to_hex(colorbar_colors(color_ind),
-                                                                    keep_alpha=True)
-            color_ind += 1
+        assert po.stretch_function.value == "arcsinh"
+        assert po.stretch_preset.value == 99
+        assert po.image_color.value == matplotlib.colors.to_hex(colorbar_colors(7-color_ind),
+                                                                keep_alpha=True)
+        color_ind += 1
 
 
 def test_track_mixed_states(imviz_helper):
     # Initialize two viewer with 3 data each.
     # Each layer of the data will be RGB
     arr = np.arange(36).reshape(6, 6)
     po = imviz_helper.app.get_tray_item_from_name("g-plot-options")
@@ -375,7 +379,46 @@
     # mixed state and are the same color
     po.image_color.unmix_state()
     assert len(po.layer.items[-1]["colors"]) == 1
     assert len(po.layer.items[-2]["colors"]) == 1
     assert po.image_color.value == "#00ff00"
     assert po.layer.items[-1]["colors"][0] == "#00ff00"
     assert po.layer.items[-2]["colors"][0] == "#00ff00"
+
+    # test spline stretch mixed state
+    po.viewer_selected = ["imviz-0"]
+    po.layer_selected = ["array_1"]
+    po.stretch_function_value = 'spline'
+    po.viewer_selected = ["imviz-0", "imviz-1"]
+    assert po.stretch_function_sync['mixed']
+
+    po.vue_unmix_state(['stretch_function', 'stretch_params'])
+    assert not po.stretch_function_sync['mixed']
+    assert po.stretch_function_value == 'spline'
+    assert not po.stretch_params_sync['mixed']
+
+
+def test_segmentation_image(imviz_helper):
+    # Make one circular segment for a hypothetical
+    # image with one source:
+    nx = ny = 100
+    radius = 15
+    x0 = y0 = 50
+
+    segmentation_map = np.zeros((nx, ny))
+    xx, yy = np.meshgrid(np.arange(nx), np.arange(ny))
+    in_circle = np.hypot(xx - x0, yy - y0) < radius
+    segmentation_map[in_circle] = 1
+
+    imviz_helper.load_data(segmentation_map)
+
+    plot_opts = imviz_helper.plugins['Plot Options']
+    plot_opts.image_colormap = 'Random'
+
+    # ensure that stretch preset is adjusted when the image segmentaiton
+    # option is selected for the "Random" colormap, so that all colors
+    # are uniquely displayed:
+    plot_opts._obj.image_segmentation_map_presets()
+    assert plot_opts.stretch_preset.value == 100
+    assert plot_opts.stretch_function.value == 'linear'
+    assert plot_opts.image_bias.value == 0.5
+    assert plot_opts.image_contrast.value == 1.0
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.py` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,20 +10,23 @@
 from glue.core.roi import CircularROI, CircularAnnulusROI, EllipticalROI, RectangularROI
 from glue.core.subset import RoiSubsetState, RangeSubsetState, CompositeSubsetState
 from glue.icons import icon_path
 from glue_jupyter.widgets.subset_mode_vuetify import SelectionModeMenu
 from glue_jupyter.common.toolbar_vuetify import read_icon
 from traitlets import Any, List, Unicode, Bool, observe
 
-from jdaviz.core.events import SnackbarMessage, GlobalDisplayUnitChanged
+from jdaviz.core.events import SnackbarMessage, GlobalDisplayUnitChanged, LinkUpdatedMessage
 from jdaviz.core.registries import tray_registry
 from jdaviz.core.template_mixin import PluginTemplateMixin, DatasetSelectMixin, SubsetSelect
 from jdaviz.core.tools import ICON_DIR
 from jdaviz.utils import MultiMaskSubsetState
 
+from jdaviz.configs.default.plugins.subset_plugin import utils
+
+
 __all__ = ['SubsetPlugin']
 
 SUBSET_MODES = {
     'replace': ReplaceMode,
     'OrState': OrMode,
     'AndState': AndMode,
     'XorState': XorMode,
@@ -72,23 +75,41 @@
 
         self.session.hub.subscribe(self, EditSubsetMessage,
                                    handler=self._sync_selected_from_state)
         self.session.hub.subscribe(self, SubsetUpdateMessage,
                                    handler=self._on_subset_update)
         self.session.hub.subscribe(self, GlobalDisplayUnitChanged,
                                    handler=self._on_display_unit_changed)
+        self.session.hub.subscribe(self, LinkUpdatedMessage,
+                                   handler=self._on_link_update)
 
         self.subset_select = SubsetSelect(self,
                                           'subset_items',
                                           'subset_selected',
                                           multiselect='multiselect',
                                           default_text="Create New")
         self.subset_states = []
         self.spectral_display_unit = None
 
+        link_type = getattr(self.app, '_link_type', None)
+        self.display_sky_coordinates = (link_type == 'wcs' and not self.multiselect)
+
+    def _on_link_update(self, *args):
+        """When linking is changed pixels<>wcs, change display units of the
+        subset plugin from pixel (for pixel linking) to sky (for WCS linking).
+        If there is an active selection in the subset plugin, push this change
+        to the UI upon link change by calling _get_subset_definition, which
+        will re-determine how to display subset information."""
+
+        link_type = getattr(self.app, '_link_type', None)
+        self.display_sky_coordinates = (link_type == 'wcs')
+
+        if self.subset_selected != self.subset_select.default_text:
+            self._get_subset_definition(*args)
+
     def _sync_selected_from_state(self, *args):
         if not hasattr(self, 'subset_select') or self.multiselect:
             # during initial init, this can trigger before the component is initialized
             return
         if self.session.edit_subset_mode.edit_subset == []:
             if self.subset_selected != self.subset_select.default_text:
                 self.subset_selected = self.subset_select.default_text
@@ -139,92 +160,122 @@
         Convert what app.get_subsets returns into something the UI of this plugin
         can display.
         """
         if self.multiselect:
             self.is_centerable = True
             return
 
+        include_sky_region = bool(self.display_sky_coordinates)
         subset_information = self.app.get_subsets(self.subset_selected,
                                                   simplify_spectral=False,
-                                                  use_display_units=True)
+                                                  use_display_units=True,
+                                                  include_sky_region=include_sky_region)
+
         _around_decimals = 6  # Avoid 30 degrees from coming back as 29.999999999999996
         if not subset_information:
             return
         if ((len(subset_information) == 1) and
                 (isinstance(subset_information[0]["subset_state"], RangeSubsetState) or
                  (isinstance(subset_information[0]["subset_state"], RoiSubsetState) and
                   isinstance(subset_information[0]["subset_state"].roi,
                              (CircularROI, RectangularROI, EllipticalROI))))):
             self.is_centerable = True
         else:
             self.is_centerable = False
 
         for spec in subset_information:
+
             subset_definition = []
             subset_type = ''
             subset_state = spec["subset_state"]
             glue_state = spec["glue_state"]
+
             if isinstance(subset_state, RoiSubsetState):
                 subset_definition.append({
                     "name": "Parent", "att": "parent",
                     "value": subset_state.xatt.parent.label,
                     "orig": subset_state.xatt.parent.label})
 
-                if isinstance(subset_state.roi, CircularROI):
-                    x, y = subset_state.roi.center()
-                    r = subset_state.roi.radius
-                    subset_definition += [
-                        {"name": "X Center", "att": "xc", "value": x, "orig": x},
-                        {"name": "Y Center", "att": "yc", "value": y, "orig": y},
-                        {"name": "Radius", "att": "radius", "value": r, "orig": r}]
-
-                elif isinstance(subset_state.roi, RectangularROI):
-                    for att in ("Xmin", "Xmax", "Ymin", "Ymax"):
-                        real_att = att.lower()
-                        val = getattr(subset_state.roi, real_att)
-                        subset_definition.append(
-                            {"name": att, "att": real_att, "value": val, "orig": val})
-                    theta = np.around(np.degrees(subset_state.roi.theta), decimals=_around_decimals)
-                    subset_definition.append(
-                        {"name": "Angle", "att": "theta", "value": theta, "orig": theta})
-
-                elif isinstance(subset_state.roi, EllipticalROI):
-                    xc, yc = subset_state.roi.center()
-                    rx = subset_state.roi.radius_x
-                    ry = subset_state.roi.radius_y
-                    theta = np.around(np.degrees(subset_state.roi.theta), decimals=_around_decimals)
-                    subset_definition += [
-                        {"name": "X Center", "att": "xc", "value": xc, "orig": xc},
-                        {"name": "Y Center", "att": "yc", "value": yc, "orig": yc},
-                        {"name": "X Radius", "att": "radius_x", "value": rx, "orig": rx},
-                        {"name": "Y Radius", "att": "radius_y", "value": ry, "orig": ry},
-                        {"name": "Angle", "att": "theta", "value": theta, "orig": theta}]
-
-                elif isinstance(subset_state.roi, CircularAnnulusROI):
-                    x, y = subset_state.roi.center()
-                    inner_r = subset_state.roi.inner_radius
-                    outer_r = subset_state.roi.outer_radius
-                    subset_definition += [{"name": "X Center", "att": "xc", "value": x, "orig": x},
-                                          {"name": "Y Center", "att": "yc", "value": y, "orig": y},
-                                          {"name": "Inner radius", "att": "inner_radius",
-                                           "value": inner_r, "orig": inner_r},
-                                          {"name": "Outer radius", "att": "outer_radius",
-                                           "value": outer_r, "orig": outer_r}]
+                sky_region = spec['sky_region']
+                if self.display_sky_coordinates and (sky_region is not None):
+                    subset_definition += utils._sky_region_to_subset_def(sky_region)
+
+                else:
+                    if isinstance(subset_state.roi, CircularROI):
+                        x, y = subset_state.roi.center()
+                        r = subset_state.roi.radius
+                        subset_definition += [
+                            {"name": "X Center (pixels)", "att": "xc",
+                             "value": x, "orig": x},
+                            {"name": "Y Center (pixels)", "att": "yc",
+                             "value": y, "orig": y},
+                            {"name": "Radius (pixels)", "att": "radius",
+                             "value": r, "orig": r}]
+
+                    elif isinstance(subset_state.roi, RectangularROI):
+                        for att in ("Xmin", "Xmax", "Ymin", "Ymax"):
+                            real_att = att.lower()
+                            val = getattr(subset_state.roi, real_att)
+                            subset_definition.append(
+                                {"name": att + " (pixels)", "att": real_att,
+                                 "value": val, "orig": val})
+
+                        theta = np.around(np.degrees(subset_state.roi.theta),
+                                          decimals=_around_decimals)
+                        subset_definition.append({"name": "Angle", "att": "theta",
+                                                  "value": theta, "orig": theta})
+
+                    elif isinstance(subset_state.roi, EllipticalROI):
+                        xc, yc = subset_state.roi.center()
+                        rx = subset_state.roi.radius_x
+                        ry = subset_state.roi.radius_y
+                        theta = np.around(np.degrees(subset_state.roi.theta),
+                                          decimals=_around_decimals)
+
+                        subset_definition += [
+                            {"name": "X Center (pixels)", "att": "xc",
+                             "value": xc, "orig": xc},
+                            {"name": "Y Center (pixels)", "att": "yc",
+                             "value": yc, "orig": yc},
+                            {"name": "X Radius (pixels)", "att": "radius_x",
+                             "value": rx, "orig": rx},
+                            {"name": "Y Radius (pixels)", "att": "radius_y",
+                             "value": ry, "orig": ry},
+                            {"name": "Angle", "att": "theta",
+                             "value": theta, "orig": theta}]
+
+                    elif isinstance(subset_state.roi, CircularAnnulusROI):
+                        xc, yc = subset_state.roi.center()
+                        inner_r = subset_state.roi.inner_radius
+                        outer_r = subset_state.roi.outer_radius
+                        subset_definition += [{"name": "X Center (pixels)",
+                                               "att": "xc", "value": xc, "orig": xc},
+                                              {"name": "Y Center (pixels)",
+                                               "att": "yc", "value": yc, "orig": yc},
+                                              {"name": "Inner Radius (pixels)",
+                                               "att": "inner_radius",
+                                               "value": inner_r, "orig": inner_r},
+                                              {"name": "Outer Radius (pixels)",
+                                               "att": "outer_radius",
+                                               "value": outer_r, "orig": outer_r}]
+
+                    else:  # pragma: no cover
+                        raise NotImplementedError(f"Unable to translate {subset_state.roi.__class__.__name__}")  # noqa: E501
 
                 subset_type = subset_state.roi.__class__.__name__
 
             elif isinstance(subset_state, RangeSubsetState):
                 region = spec['region']
                 if isinstance(region, Time):
                     lo = region.min()
                     hi = region.max()
-                    subset_definition = [{"name": "Lower bound", "att": "lo", "value": lo.value,
-                                          "orig": lo.value},
-                                         {"name": "Upper bound", "att": "hi", "value": hi.value,
-                                          "orig": hi.value}]
+                    subset_definition = [{"name": "Lower bound", "att": "lo",
+                                          "value": lo.value, "orig": lo.value},
+                                         {"name": "Upper bound", "att": "hi",
+                                          "value": hi.value, "orig": hi.value}]
                 else:
                     lo = region.lower
                     hi = region.upper
                     subset_definition = [{"name": "Lower bound", "att": "lo", "value": lo.value,
                                           "orig": lo.value, "unit": str(lo.unit)},
                                          {"name": "Upper bound", "att": "hi", "value": hi.value,
                                           "orig": hi.value, "unit": str(hi.unit)}]
@@ -240,17 +291,17 @@
                 # Note: .append() does not work for List traitlet.
                 self.subset_definitions = self.subset_definitions + [subset_definition]
                 self.subset_types = self.subset_types + [subset_type]
                 self.glue_state_types = self.glue_state_types + [glue_state]
                 self.subset_states = self.subset_states + [subset_state]
 
         simplifiable_states = set(['AndState', 'XorState', 'AndNotState'])
-        # Check if the subset has more than one subregion, is a range subset type, and
-        # uses one of the states that can be simplified. Mask subset types cannot be simplified
-        # so subsets contained that are skipped.
+        # Check if the subset has more than one subregion, is a range subset
+        # type, and uses one of the states that can be simplified. Mask subset
+        # types cannot be simplified so subsets contained that are skipped.
         if 'Mask' in self.subset_types:
             self.can_simplify = False
         elif (len(self.subset_states) > 1 and isinstance(self.subset_states[0], RangeSubsetState)
                 and len(simplifiable_states - set(self.glue_state_types)) < 3):
             self.can_simplify = True
         elif (len(self.subset_states) > 1 and isinstance(self.subset_states[0], RangeSubsetState)
               and self.app.is_there_overlap_spectral_subset(self.subset_selected)):
@@ -299,14 +350,15 @@
         # We only care about the spectral units, since flux units don't affect spectral subsets
         if msg.axis == "spectral":
             self.spectral_display_unit = msg.unit
             if self.subset_selected != self.subset_select.default_text:
                 self._get_subset_definition(self.subset_selected)
 
     def vue_update_subset(self, *args):
+
         if self.multiselect:
             self.hub.broadcast(SnackbarMessage("Cannot update subset "
                                                "when multiselect is active", color='warning',
                                                sender=self))
             return
 
         status, reason = self._check_input()
@@ -314,19 +366,40 @@
             self.hub.broadcast(SnackbarMessage(reason, color='error', sender=self))
             return
 
         for index, sub in enumerate(self.subset_definitions):
             if len(self.subset_states) <= index:
                 return
             sub_states = self.subset_states[index]
+
+            # we need to push updates to subset in pixels. to do this when wcs
+            # linked, convert the updated subset parameters from sky to pix
+            wcs = None
+
+            if self.display_sky_coordinates:
+                wcs = self.app._get_wcs_from_subset(sub_states)
+
+                if wcs is not None:
+                    # convert newly entered sky coords to pixel
+                    updated_skyreg = utils._subset_def_to_region(self.subset_types[index], sub)  # noqa
+                    updated_pixreg_attrs = utils._get_pixregion_params_in_dict(updated_skyreg.to_pixel(wcs))  # noqa
+                    # convert previous entered sky coords to pixel
+                    orig_skyreg = utils._subset_def_to_region(self.subset_types[index], sub, val='orig')  # noqa
+                    orig_pixreg_attrs = utils._get_pixregion_params_in_dict(orig_skyreg.to_pixel(wcs))  # noqa
+
             for d_att in sub:
                 if d_att["att"] == 'parent':  # Read-only
                     continue
-
-                if d_att["att"] == 'theta':  # Humans use degrees but glue uses radians
+                if self.display_sky_coordinates and (wcs is not None):
+                    d_att["value"] = updated_pixreg_attrs[d_att["att"]]
+                    d_att["orig"] = orig_pixreg_attrs[d_att["att"]]
+
+                if (d_att["att"] == 'theta') and (self.display_sky_coordinates is False):
+                    # Humans use degrees but glue uses radians
+                    # We've already enforced this in wcs linking in _get_pixregion_params_in_dict
                     d_val = np.radians(d_att["value"])
                 else:
                     d_val = float(d_att["value"])
 
                 # Convert from display unit to original unit if necessary
                 if self.subset_types[index] == "Range":
                     if self.spectral_display_unit is not None:
@@ -338,14 +411,15 @@
                             d_val = d_val.value
 
                 if float(d_att["orig"]) != d_val:
                     if self.subset_types[index] == "Range":
                         setattr(sub_states, d_att["att"], d_val)
                     else:
                         setattr(sub_states.roi, d_att["att"], d_val)
+
         self._push_update_to_ui()
 
     def _push_update_to_ui(self, subset_name=None):
         """
         Forces the UI to update how it represents the subset.
 
         Parameters
@@ -418,15 +492,15 @@
 
         from astropy.wcs.utils import pixel_to_pixel
         from photutils.aperture import ApertureStats
         from jdaviz.core.region_translators import regions2aperture, _get_region_from_spatial_subset
 
         def _do_recentering(subset, subset_state):
             try:
-                reg = _get_region_from_spatial_subset(self, subset_state) # noqa
+                reg = _get_region_from_spatial_subset(self, subset_state)
                 aperture = regions2aperture(reg)
                 data = self.dataset.selected_dc_item
                 comp = data.get_component(data.main_components[0])
                 comp_data = comp.data
                 phot_aperstats = ApertureStats(comp_data, aperture, wcs=data.coords)
 
                 # Sky region from WCS linking, need to convert centroid back to pixels.
@@ -435,15 +509,14 @@
                     # However, Subset is always defined w.r.t. its parent,
                     # so we need to convert back.
                     x, y = pixel_to_pixel(
                         data.coords,
                         subset_state.xatt.parent.coords,
                         phot_aperstats.xcentroid,
                         phot_aperstats.ycentroid)
-
                 else:
                     x = phot_aperstats.xcentroid
                     y = phot_aperstats.ycentroid
                 if not np.all(np.isfinite((x, y))):
                     raise ValueError(f'Invalid centroid ({x}, {y})')
             except Exception as err:
                 self.set_center(self.get_center(subset_name=subset), subset_name=subset,
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.vue` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.vue`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 <template>
   <j-tray-plugin
-    description='Tools for selecting and interacting with subsets.'
+    :description="docs_description || 'Tools for selecting and interacting with subsets.'"
     :link="docs_link || 'https://jdaviz.readthedocs.io/en/'+vdocs+'/'+config+'/plugins.html#subset-tools'"
-    :popout_button="popout_button">
+    :popout_button="popout_button"
+    :scroll_to.sync="scroll_to">
 
     <v-row v-if="config === 'imviz'">
       <div style="width: calc(100% - 32px)">
       </div>
       <div style="width: 32px">
         <j-tooltip tooltipcontent="Multiselect for recentering subsets">
           <v-btn
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/subset_tools/subset_tools.py` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/subset_tools/subset_tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.py` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.vue` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/default/plugins/viewers.py` & `jdaviz-3.9.0/jdaviz/configs/default/plugins/viewers.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from glue_jupyter.table import TableViewer
 
 from jdaviz.configs.imviz.helper import layer_is_image_data
 from jdaviz.components.toolbar_nested import NestedJupyterToolbar
 from jdaviz.core.astrowidgets_api import AstrowidgetsImageViewerMixin
 from jdaviz.core.registries import viewer_registry
 from jdaviz.core.user_api import ViewerUserApi
-from jdaviz.utils import ColorCycler, get_subset_type
+from jdaviz.utils import ColorCycler, get_subset_type, _wcs_only_label
 
 __all__ = ['JdavizViewerMixin']
 
 viewer_registry.add("g-profile-viewer", label="Profile 1D", cls=BqplotProfileView)
 viewer_registry.add("g-image-viewer", label="Image 2D", cls=BqplotImageView)
 viewer_registry.add("g-table-viewer", label="Table", cls=TableViewer)
 
@@ -32,33 +32,66 @@
 
         # Allow each viewer to cycle through colors for each new addition to the viewer:
         self.color_cycler = ColorCycler()
 
     @property
     def user_api(self):
         # default exposed user APIs.  Can override this method in any particular viewer.
+        if not isinstance(self, TableViewer):
+            expose = ['data_labels', 'data_labels_loaded', 'data_labels_visible']
+        else:
+            expose = []
         if isinstance(self, BqplotImageView):
             if isinstance(self, AstrowidgetsImageViewerMixin):
-                expose = ['save',
-                          'center_on', 'offset_by', 'zoom_level', 'zoom',
-                          'colormap_options', 'set_colormap',
-                          'stretch_options', 'stretch',
-                          'autocut_options', 'cuts',
-                          'marker', 'add_markers', 'remove_markers', 'reset_markers',
-                          'blink_once', 'reset_limits']
+                expose += ['save',
+                           'center_on', 'offset_by', 'zoom_level', 'zoom',
+                           'colormap_options', 'set_colormap',
+                           'stretch_options', 'stretch',
+                           'autocut_options', 'cuts',
+                           'marker', 'add_markers', 'remove_markers', 'reset_markers',
+                           'blink_once', 'reset_limits']
             else:
                 # cubeviz image viewers don't inherit from AstrowidgetsImageViewerMixin yet,
                 # but also shouldn't expose set_limits because of equal aspect ratio concerns
-                expose = []
+                expose += []
         elif isinstance(self, TableViewer):
-            expose = []
+            expose += []
         else:
-            expose = ['set_limits', 'reset_limits']
+            expose += ['set_limits', 'reset_limits']
         return ViewerUserApi(self, expose=expose)
 
+    @property
+    def data_labels_loaded(self):
+        """
+        List of data labels loaded in this viewer.
+
+        Returns
+        -------
+        data_labels : list
+            list of strings
+        """
+        viewer_item = self.jdaviz_app._get_viewer_item(self.reference_id)
+        return [self.jdaviz_app._get_data_item_by_id(data_id)['name']
+                for data_id in viewer_item.get('selected_data_items', {}).keys()]
+
+    @property
+    def data_labels_visible(self):
+        """
+        List of data labels visible in this viewer.
+
+        Returns
+        -------
+        data_labels : list
+            list of strings
+        """
+        viewer_item = self.jdaviz_app._get_viewer_item(self.reference_id)
+        return [self.jdaviz_app._get_data_item_by_id(data_id)['name']
+                for data_id, visibility in viewer_item.get('selected_data_items', {}).items()
+                if visibility != 'hidden']
+
     def reset_limits(self):
         """
         Reset viewer axes limits.
         """
         self.state.reset_limits()
 
     def set_limits(self, x_min=None, x_max=None, y_min=None, y_max=None):
@@ -176,15 +209,19 @@
                         return "mdi-chart-scatter-plot", suffix
                     else:
                         return "mdi-chart-bell-curve", ""
             return "", suffix
 
         visible_layers = {}
         for layer in self.state.layers[::-1]:
-            if layer.visible:
+            layer_is_wcs_only = (
+                    hasattr(layer.layer, 'meta') and
+                    layer.layer.meta.get(_wcs_only_label, False)
+            )
+            if layer.visible and not layer_is_wcs_only:
                 prefix_icon, suffix = _get_layer_info(layer)
                 visible_layers[layer.layer.label] = {'color': _get_layer_color(layer),
                                                      'linewidth': _get_layer_linewidth(layer),
                                                      'prefix_icon': prefix_icon,
                                                      'suffix_label': suffix}
 
         viewer_item = self.jdaviz_app._viewer_item_by_id(self.reference_id)
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/helper.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/helper.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,32 +2,27 @@
 import re
 import warnings
 from copy import deepcopy
 
 import numpy as np
 from glue.core import BaseData
 from glue.core.link_helpers import LinkSame
-from glue.plugins.wcs_autolinking.wcs_autolinking import WCSLink, NoAffineApproximation
 
-from jdaviz.core.events import SnackbarMessage, NewViewerMessage, LinkUpdatedMessage
+from jdaviz.core.events import SnackbarMessage, NewViewerMessage
 from jdaviz.core.helpers import ImageConfigHelper
+from jdaviz.utils import data_has_valid_wcs, _wcs_only_label
 
-__all__ = ['Imviz', 'link_image_data']
+__all__ = ['Imviz']
 
 
 class Imviz(ImageConfigHelper):
     """Imviz Helper class."""
     _default_configuration = 'imviz'
     _default_viewer_reference_name = "image-viewer"
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.app._link_type = None
-        self.app._wcs_use_affine = None
-
     def create_image_viewer(self, viewer_name=None):
         """Create a new image viewer.
 
         To display data in this new viewer programmatically,
         first get the new viewer ID from the small tab on the top
         left of viewer display. Then, use
         :meth:`~jdaviz.app.Application.add_data_to_viewer` from ``imviz.app``
@@ -47,17 +42,22 @@
             Image viewer instance.
 
         """
         from jdaviz.configs.imviz.plugins.viewers import ImvizImageView
 
         # Cannot assign data to real Data because it loads but it will
         # not update checkbox in Data menu.
+
+        # add WCS-only layers from all viewers into the new viewer
+        add_layers_to_viewer = get_wcs_only_layer_labels(self.app)
+
         return self.app._on_new_viewer(
             NewViewerMessage(ImvizImageView, data=None, sender=self.app),
-            vid=viewer_name, name=viewer_name)
+            vid=viewer_name, name=viewer_name,
+            add_layers_to_viewer=add_layers_to_viewer)
 
     def destroy_viewer(self, viewer_id):
         """Destroy a viewer associated with the given ID.
 
         Raises
         ------
         ValueError
@@ -141,15 +141,14 @@
                     kw['ext'] = ext
 
                 # This will only overwrite if not provided.
                 if not data_label:
                     kw['data_label'] = None
                 else:
                     kw['data_label'] = data_label
-
                 self.app.load_data(filepath, parser_reference='imviz-data-parser', **kw)
 
         elif isinstance(data, np.ndarray) and data.ndim >= 3:
             if data.ndim > 3:
                 data = data.squeeze()
                 if data.ndim != 3:
                     raise ValueError(f'Imviz cannot load this array with ndim={data.ndim}')
@@ -171,43 +170,90 @@
         else:
             if data_label:
                 kwargs['data_label'] = data_label
             self.app.load_data(data, parser_reference='imviz-data-parser', **kwargs)
 
         # find the current label(s) - TODO: replace this by calling default label functionality
         # above instead of having to refind it
-        applied_labels = [label for label in self.app.data_collection.labels if label not in prev_data_labels]  # noqa
+        applied_labels = []
+        applied_visible = []
+        layer_is_wcs_only = []
+        layer_has_wcs = []
+        for data in self.app.data_collection:
+            label = data.label
+            if label not in prev_data_labels:
+                applied_labels.append(label)
+                applied_visible.append(True)
+                layer_is_wcs_only.append(data.meta.get(_wcs_only_label, False))
+                layer_has_wcs.append(data_has_valid_wcs(data))
 
         if show_in_viewer is True:
             show_in_viewer = f"{self.app.config}-0"
 
+        if show_in_viewer:
+            linked_by_wcs = self.app._link_type == 'wcs'
+            if linked_by_wcs:
+                for applied_label, visible, is_wcs_only, has_wcs in zip(
+                        applied_labels, applied_visible, layer_is_wcs_only, layer_has_wcs
+                ):
+                    if not is_wcs_only and linked_by_wcs and not has_wcs:
+                        self.app.hub.broadcast(SnackbarMessage(
+                            f"'{applied_label}' will be added to the data collection but not "
+                            f"the viewer '{show_in_viewer}', since data are linked by WCS, but "
+                            f"'{applied_label}' has no WCS.",
+                            color="warning", timeout=8000, sender=self)
+                        )
+
         if self._in_batch_load and show_in_viewer:
-            for applied_label in applied_labels:
-                self._delayed_show_in_viewer_labels[applied_label] = show_in_viewer
+            for applied_label, is_wcs_only in zip(applied_labels, layer_is_wcs_only):
+                if not is_wcs_only:
+                    self._delayed_show_in_viewer_labels[applied_label] = show_in_viewer
 
         else:
-            if 'Links Control' not in self.plugins.keys():
+            if 'Orientation' not in self.plugins.keys():
                 # otherwise plugin will handle linking automatically with DataCollectionAddMessage
-                self.link_data(link_type='pixels', error_on_fail=False)
+                self.link_data(link_type='wcs')
 
             # One input might load into multiple Data objects.
             # NOTE: If the batch_load context manager was used, it will
             # handle that logic instead.
             if show_in_viewer:
-                for applied_label in applied_labels:
-                    self.app.add_data_to_viewer(show_in_viewer, applied_label)
+                for applied_label, visible, has_wcs in zip(
+                        applied_labels, applied_visible, layer_has_wcs
+                ):
+                    if (has_wcs and linked_by_wcs) or not linked_by_wcs:
+                        self.app.add_data_to_viewer(show_in_viewer, applied_label, visible=visible)
 
-    def link_data(self, **kwargs):
+    def link_data(self, link_type='pixels', wcs_fallback_scheme=None, wcs_use_affine=True):
         """(Re)link loaded data in Imviz with the desired link type.
         All existing links will be replaced.
 
-        See :func:`~jdaviz.configs.imviz.helper.link_image_data`
-        for available keyword options and more details.
+        Parameters
+        ----------
+        link_type : {'pixels', 'wcs'}
+            Choose to link by pixels or WCS.
+
+        wcs_fallback_scheme : {None, 'pixels'}
+            If WCS linking failed, choose to fall back to linking by pixels or not at all.
+            This is only used when ``link_type='wcs'``.
+            Choosing `None` may result in some Imviz functionality not working properly.
+
+        wcs_use_affine : bool
+            Use an affine transform to represent the offset between images if possible
+            (requires that the approximation is accurate to within 1 pixel with the
+            full WCS transformations). If approximation fails, it will automatically
+            fall back to full WCS transformation. This is only used when ``link_type='wcs'``.
+            Affine approximation is much more performant at the cost of accuracy.
+
         """
-        link_image_data(self.app, **kwargs)
+        from jdaviz.configs.imviz.plugins.orientation.orientation import link_type_msg_to_trait
+        plg = self.plugins["Orientation"]
+        plg._obj.wcs_use_fallback = wcs_fallback_scheme == 'pixels'
+        plg.wcs_use_affine = wcs_use_affine
+        plg.link_type = link_type_msg_to_trait[link_type]
 
     def get_link_type(self, data_label_1, data_label_2):
         """Find the type of ``glue`` linking between the given
         data labels. A link is bi-directional. If there are
         more than 2 data in the collection, one of the given
         labels should be the reference data or look-up will fail.
 
@@ -215,15 +261,15 @@
         ----------
         data_label_1, data_label_2 : str
            Labels for the data linked together.
 
         Returns
         -------
         link_type : {'pixels', 'wcs', 'self'}
-            One of the link types accepted by :func:`~jdaviz.configs.imviz.helper.link_image_data`
+            One of the link types accepted by the Orientation plugin
             or ``'self'`` if the labels are identical.
 
         Raises
         ------
         ValueError
             Link look-up failed.
 
@@ -238,16 +284,18 @@
                 if isinstance(elink, LinkSame):  # Assumes WCS link never uses LinkSame
                     link_type = 'pixels'
                 else:  # If not pixels, must be WCS
                     link_type = 'wcs'
                 break  # Might have duplicate, just grab first match
 
         if link_type is None:
+            avail_links = [f"({elink.data1.label}, {elink.data2.label})"
+                           for elink in self.app.data_collection.external_links]
             raise ValueError(f'{data_label_1} and {data_label_2} combo not found '
-                             'in data collection external links')
+                             f'in data collection external links: {avail_links}')
 
         return link_type
 
     def get_aperture_photometry_results(self):
         """Return aperture photometry results, if any.
         Results are calculated using :ref:`aper-phot-simple` plugin.
 
@@ -340,191 +388,57 @@
 
     filepath = f'{s[0]}{sfx}'
     data_label = os.path.basename(s[0])
 
     return filepath, ext, data_label
 
 
-def layer_is_image_data(layer):
+def layer_is_2d(layer):
+    # returns True for subclasses of BaseData with ndim=2, both for
+    # layers that are WCS-only as well as images containing data:
     return isinstance(layer, BaseData) and layer.ndim == 2
 
 
-def layer_is_table_data(layer):
-    return isinstance(layer, BaseData) and layer.ndim == 1
+def layer_is_image_data(layer):
+    return layer_is_2d(layer) and not layer.meta.get(_wcs_only_label, False)
+
+
+def layer_is_wcs_only(layer):
+    return layer_is_2d(layer) and layer.meta.get(_wcs_only_label, False)
+
+
+def get_wcs_only_layer_labels(app):
+    return [data.label for data in app.data_collection
+            if layer_is_wcs_only(data)]
 
 
 def get_top_layer_index(viewer):
     """Get index of the top visible image layer in Imviz.
     This is because when blinked, first layer might not be top visible layer.
 
     """
-    return [i for i, lyr in enumerate(viewer.layers)
-            if lyr.visible and layer_is_image_data(lyr.layer)][-1]
-
-
-def get_reference_image_data(app):
-    """Return the first 2D image data in collection and its index to use as reference."""
-    refdata = None
-    iref = 0
-    for i, data in enumerate(app.data_collection):
-        if layer_is_image_data(data):
-            iref = i
-            refdata = data
-            break
-    if refdata is None:
-        raise ValueError(f'No valid reference data found in collection: {app.data_collection}')
-    return refdata, iref
-
-
-def link_image_data(app, link_type='pixels', wcs_fallback_scheme='pixels', wcs_use_affine=True,
-                    error_on_fail=False, update_plugin=True):
-    """(Re)link loaded data in Imviz with the desired link type.
-    All existing links will be replaced.
-
-    .. note::
-
-        Any markers added in Imviz will need to be removed manually before changing linking type.
-        You can add back the markers using
-        :meth:`~jdaviz.core.astrowidgets_api.AstrowidgetsImageViewerMixin.add_markers`
-        for the relevant viewer(s).
-
-    Parameters
-    ----------
-    app : `~jdaviz.app.Application`
-        Application associated with Imviz, e.g., ``imviz.app``.
+    visible_image_layers = [
+        i for i, lyr in enumerate(viewer.layers)
+        if lyr.visible and layer_is_image_data(lyr.layer)
+    ]
 
-    link_type : {'pixels', 'wcs'}
-        Choose to link by pixels or WCS.
+    if len(visible_image_layers):
+        return visible_image_layers[-1]
+    return None
 
-    wcs_fallback_scheme : {None, 'pixels'}
-        If WCS linking failed, choose to fall back to linking by pixels or not at all.
-        This is only used when ``link_type='wcs'``.
-        Choosing `None` may result in some Imviz functionality not working properly.
-
-    wcs_use_affine : bool
-        Use an affine transform to represent the offset between images if possible
-        (requires that the approximation is accurate to within 1 pixel with the
-        full WCS transformations). If approximation fails, it will automatically
-        fall back to full WCS transformation. This is only used when ``link_type='wcs'``.
-        Affine approximation is much more performant at the cost of accuracy.
-
-    error_on_fail : bool
-        If `True`, any failure in linking will raise an exception.
-        If `False`, warnings will be emitted as snackbar messages.
-        When only warnings are emitted and no links are assigned,
-        some Imviz functionality may not work properly.
-
-    update_plugin : bool
-        Whether to update the state of the "Links Control" plugin, if available.
-
-    Raises
-    ------
-    ValueError
-        Invalid inputs or reference data.
 
+def get_reference_image_data(app, viewer_id=None):
     """
-    if len(app.data_collection) <= 1:  # No need to link, we are done.
-        return
-
-    if link_type not in ('pixels', 'wcs'):
-        raise ValueError(f"link_type must be 'pixels' or 'wcs', got {link_type}")
-    if link_type == 'wcs' and wcs_fallback_scheme not in (None, 'pixels'):
-        raise ValueError("wcs_fallback_scheme must be None or 'pixels', "
-                         f"got {wcs_fallback_scheme}")
-
-    # if the plugin exists, send a message so that the plugin's state is updated and spinner
-    # is shown (the plugin will make a call back here)
-    if 'imviz-links-control' in [item['name'] for item in app.state.tray_items]:
-        link_plugin = app.get_tray_item_from_name('imviz-links-control')
-        if update_plugin:
-            link_plugin.linking_in_progress = True
+    Return the current reference data in the given image viewer and its index.
+    By default, the first viewer is used.
+    """
+    if viewer_id is None:
+        refdata = app._jdaviz_helper.default_viewer._obj.state.reference_data
     else:
-        link_plugin = None
+        viewer = app.get_viewer_by_id(viewer_id)
+        refdata = viewer.state.reference_data
 
-    if link_type == app._link_type and wcs_use_affine == app._wcs_use_affine:
-        data_already_linked = [link.data2 for link in app.data_collection.external_links]
-    else:
-        for viewer in app._viewer_store.values():
-            if len(viewer._marktags):
-                raise ValueError(f"cannot change link_type (from '{app._link_type}' to "
-                                 f"'{link_type}') when markers are present. "
-                                 f" Clear markers with viewer.reset_markers() first")
-        data_already_linked = []
-
-    refdata, iref = get_reference_image_data(app)
-    links_list = []
-    ids0 = refdata.pixel_component_ids
-    ndim_range = range(refdata.ndim)
-
-    for i, data in enumerate(app.data_collection):
-        # Do not link with self
-        if i == iref:
-            continue
-
-        # We are not touching any existing Subsets. They keep their own links.
-        if not layer_is_image_data(data):
-            continue
-
-        if data in data_already_linked:
-            # links already exist for this entry and we're not changing the type
-            continue
-
-        ids1 = data.pixel_component_ids
-        try:
-            if link_type == 'pixels':
-                new_links = [LinkSame(ids0[i], ids1[i]) for i in ndim_range]
-            else:  # 'wcs'
-                wcslink = WCSLink(data1=refdata, data2=data, cids1=ids0, cids2=ids1)
-                if wcs_use_affine:
-                    try:
-                        new_links = [wcslink.as_affine_link()]
-                    except NoAffineApproximation:  # pragma: no cover
-                        new_links = [wcslink]
-                else:
-                    new_links = [wcslink]
-        except Exception as e:
-            if link_type == 'wcs' and wcs_fallback_scheme == 'pixels':
-                try:
-                    new_links = [LinkSame(ids0[i], ids1[i]) for i in ndim_range]
-                except Exception as e:  # pragma: no cover
-                    if error_on_fail:
-                        raise
-                    else:
-                        app.hub.broadcast(SnackbarMessage(
-                            f"Error linking '{data.label}' to '{refdata.label}': "
-                            f"{repr(e)}", color="warning", timeout=8000, sender=app))
-                        continue
-            else:
-                if error_on_fail:
-                    raise
-                else:
-                    app.hub.broadcast(SnackbarMessage(
-                        f"Error linking '{data.label}' to '{refdata.label}': "
-                        f"{repr(e)}", color="warning", timeout=8000, sender=app))
-                    continue
-        links_list += new_links
-
-    if len(links_list) > 0:
-        with app.data_collection.delay_link_manager_update():
-            if len(data_already_linked):
-                app.data_collection.add_link(links_list)
-            else:
-                app.data_collection.set_links(links_list)
-
-        app.hub.broadcast(SnackbarMessage(
-            'Images successfully relinked', color='success', timeout=8000, sender=app))
-
-    app._link_type = link_type
-    app._wcs_use_affine = wcs_use_affine
-
-    if link_plugin is not None:
-        # Only broadcast after success.
-        app.hub.broadcast(LinkUpdatedMessage(link_type,
-                                             wcs_fallback_scheme == 'pixels',
-                                             wcs_use_affine,
-                                             sender=app))
-        # reset the progress spinner
-        link_plugin.linking_in_progress = False
-
-    for viewer in app._viewer_store.values():
-        # viewer-state needs to know link type for reset_limits behavior
-        viewer.state.linked_by_wcs = link_type == 'wcs'
+    if refdata is not None:
+        iref = app.data_collection.index(refdata)
+        return refdata, iref
+
+    return None, -1
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/imviz.ipynb` & `jdaviz-3.9.0/jdaviz/configs/imviz/imviz.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/imviz.yaml` & `jdaviz-3.9.0/jdaviz/configs/imviz/imviz.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 toolbar:
   - g-data-tools
   - g-subset-tools
   - g-image-viewer-creator
   - g-coords-info
 tray:
   - g-metadata-viewer
+  - imviz-orientation
   - g-plot-options
   - g-subset-plugin
   - g-markers
-  - imviz-links-control
   - imviz-compass
   - imviz-line-profile-xy
   - imviz-aper-phot-simple
   - imviz-catalogs
   - imviz-footprints
   - imviz-rotate-canvas
-  - g-export-plot
+  - export
 viewer_area:
   - container: col
     children:
       - container: row
         viewers:
           - name: imviz-0
             plot: imviz-image-viewer
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,53 +6,51 @@
 import numpy as np
 from astropy import units as u
 from astropy.modeling.fitting import LevMarLSQFitter
 from astropy.modeling import Parameter
 from astropy.modeling.models import Gaussian1D
 from astropy.time import Time
 from glue.core.message import SubsetUpdateMessage
-from glue_jupyter.common.toolbar_vuetify import read_icon
 from ipywidgets import widget_serialization
 from packaging.version import Version
 from photutils.aperture import (ApertureStats, CircularAperture, EllipticalAperture,
                                 RectangularAperture)
 from traitlets import Any, Bool, Integer, List, Unicode, observe
 
 from jdaviz.core.custom_traitlets import FloatHandleEmpty
-from jdaviz.core.events import SnackbarMessage, LinkUpdatedMessage
+from jdaviz.core.events import SnackbarMessage, LinkUpdatedMessage, SliceValueUpdatedMessage
 from jdaviz.core.region_translators import regions2aperture, _get_region_from_spatial_subset
 from jdaviz.core.registries import tray_registry
 from jdaviz.core.template_mixin import (PluginTemplateMixin, DatasetMultiSelectMixin,
-                                        SubsetSelect, TableMixin, PlotMixin, with_spinner)
-from jdaviz.core.tools import ICON_DIR
+                                        SubsetSelect, ApertureSubsetSelectMixin,
+                                        TableMixin, PlotMixin, MultiselectMixin, with_spinner)
 from jdaviz.utils import PRIHDR_KEY
 
 __all__ = ['SimpleAperturePhotometry']
 
 ASTROPY_LT_5_2 = Version(astropy.__version__) < Version('5.2')
 
 
 @tray_registry('imviz-aper-phot-simple', label="Aperture Photometry")
-class SimpleAperturePhotometry(PluginTemplateMixin, DatasetMultiSelectMixin, TableMixin, PlotMixin):
+class SimpleAperturePhotometry(PluginTemplateMixin, ApertureSubsetSelectMixin,
+                               DatasetMultiSelectMixin, TableMixin, PlotMixin, MultiselectMixin):
     """
     The Aperture Photometry plugin performs aperture photometry for drawn regions.
     See the :ref:`Aperture Photometry Plugin Documentation <aper-phot-simple>` for more details.
 
     Only the following attributes and methods are available through the
     :ref:`public plugin API <plugin-apis>`:
 
     * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.show`
-    * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.open_in_tray`
+    * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.open_in_tray`
     * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.close_in_tray`
     """
     template_file = __file__, "aper_phot_simple.vue"
-    multiselect = Bool(False).tag(sync=True)
+    uses_active_status = Bool(True).tag(sync=True)
 
-    aperture_items = List([]).tag(sync=True)
-    aperture_selected = Any('').tag(sync=True)
     aperture_area = Integer().tag(sync=True)
     background_items = List().tag(sync=True)
     background_selected = Unicode("").tag(sync=True)
     background_value = FloatHandleEmpty(0).tag(sync=True)
     pixel_area_multi_auto = Bool(True).tag(sync=True)
     pixel_area = FloatHandleEmpty(0).tag(sync=True)
     counts_factor = FloatHandleEmpty(0).tag(sync=True)
@@ -65,28 +63,21 @@
     plot_types = List([]).tag(sync=True)
     current_plot_type = Unicode().tag(sync=True)
     plot_available = Bool(False).tag(sync=True)
     radial_plot = Any('').tag(sync=True, **widget_serialization)
     fit_radial_profile = Bool(False).tag(sync=True)
     fit_results = List().tag(sync=True)
 
-    icon_radialtocheck = Unicode(read_icon(os.path.join(ICON_DIR, 'radialtocheck.svg'), 'svg+xml')).tag(sync=True)  # noqa
-    icon_checktoradial = Unicode(read_icon(os.path.join(ICON_DIR, 'checktoradial.svg'), 'svg+xml')).tag(sync=True)  # noqa
+    # Cubeviz only
+    cube_slice = Unicode("").tag(sync=True)
+    is_cube = Bool(False).tag(sync=True)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-        self.aperture = SubsetSelect(self,
-                                     'aperture_items',
-                                     'aperture_selected',
-                                     multiselect='multiselect',
-                                     dataset='dataset',
-                                     default_text=None,
-                                     filters=['is_spatial', 'is_not_composite', 'is_not_annulus'])
-
         self.background = SubsetSelect(self,
                                        'background_items',
                                        'background_selected',
                                        dataset='dataset',
                                        default_text='Manual',
                                        manual_options=['Manual'],
                                        filters=['is_spatial', 'is_not_composite'])
@@ -110,23 +101,56 @@
         self.plot.figure.fig_margin = {'top': 60, 'bottom': 60, 'left': 65, 'right': 15}
         self.plot.viewer.axis_y.tick_format = '0.2e'
         self.plot.viewer.axis_y.label_offset = '55px'
 
         self.session.hub.subscribe(self, SubsetUpdateMessage, handler=self._on_subset_update)
         self.session.hub.subscribe(self, LinkUpdatedMessage, handler=self._on_link_update)
 
+        # Custom dataset filters for Cubeviz
+        if self.config == "cubeviz":
+            def valid_cubeviz_datasets(data):
+                comp = data.get_component(data.main_components[0])
+                img_unit = u.Unit(comp.units) if comp.units else u.dimensionless_unscaled
+                acceptable_types = ['spectral flux density wav',
+                                    'photon flux density wav',
+                                    'spectral flux density',
+                                    'photon flux density']
+                return ((data.ndim in (2, 3)) and
+                        ((img_unit == (u.MJy / u.sr)) or
+                         (img_unit.physical_type in acceptable_types)))
+
+            self.dataset.add_filter(valid_cubeviz_datasets)
+            self.session.hub.subscribe(self, SliceValueUpdatedMessage,
+                                       handler=self._on_slice_changed)
+
 # TODO: expose public API once finalized
 #    @property
 #    def user_api(self):
 #        return PluginUserApi(self, expose=('multiselect', 'dataset', 'aperture',
 #                                           'background', 'background_value',
 #                                           'pixel_area', 'counts_factor', 'flux_scaling',
 #                                           'calculate_photometry',
 #                                           'unpack_batch_options', 'calculate_batch_photometry'))
 
+    def _on_slice_changed(self, msg):
+        if self.config != "cubeviz":
+            return
+        self.cube_slice = f"{msg.value:.3e} {msg.value_unit}"
+        self._cube_wave = u.Quantity(msg.value, msg.value_unit)
+
+    @observe("dataset_selected")
+    def _on_dataset_selected_changed(self, event={}):
+        if self.config != "cubeviz":
+            return
+        # self.dataset might not exist when app is setting itself up.
+        if hasattr(self, "dataset") and self.dataset.selected_dc_item.ndim > 2:
+            self.is_cube = True
+        else:
+            self.is_cube = False
+
     def _get_defaults_from_metadata(self, dataset=None):
         defaults = {}
         if dataset is None:
             meta = self.dataset.selected_dc_item.meta.copy()
         else:
             meta = self.dataset._get_dc_item(dataset).meta.copy()
 
@@ -135,19 +159,25 @@
             meta.update(meta[PRIHDR_KEY])
             del meta[PRIHDR_KEY]
         if 'telescope' in meta:
             telescope = meta['telescope']
         else:
             telescope = meta.get('TELESCOP', '')
         if telescope == 'JWST':
+            # Hardcode the flux conversion factor from MJy to ABmag
+            mjy2abmag = 0.003631
             if 'photometry' in meta and 'pixelarea_arcsecsq' in meta['photometry']:
                 defaults['pixel_area'] = meta['photometry']['pixelarea_arcsecsq']
                 if 'bunit_data' in meta and meta['bunit_data'] == u.Unit("MJy/sr"):
-                    # Hardcode the flux conversion factor from MJy to ABmag
-                    defaults['flux_scaling'] = 0.003631
+                    defaults['flux_scaling'] = mjy2abmag
+            elif 'PIXAR_A2' in meta:
+                defaults['pixel_area'] = meta['PIXAR_A2']
+                if 'BUNIT' in meta and meta['BUNIT'] == u.Unit("MJy/sr"):
+                    defaults['flux_scaling'] = mjy2abmag
+
         elif telescope == 'HST':
             # TODO: Add more HST support, as needed.
             # HST pixel scales are from instrument handbooks.
             # This is really not used because HST data does not have sr in unit.
             # This is only for completeness.
             # For counts conversion, PHOTFLAM is used to convert "counts" to flux manually,
             # which is the opposite of JWST, so we just do not do it here.
@@ -245,14 +275,17 @@
         if self.multiselect is not isinstance(self.aperture_selected, list):
             # then multiselect is in the process of changing but the traitlet for aperture_selected
             # has not been updated internally yet
             return
         if self.multiselect:
             self._background_selected_changed()
             return
+        # NOTE: aperture_selected can be triggered here before aperture_selected_validity is updated
+        # so we'll still allow the snackbar to be raised as a second warning to the user and to
+        # avoid acting on outdated information
 
         # NOTE: aperture area is only used to determine if a warning should be shown in the UI
         # and so does not need to be calculated within user API calls that don't act on traitlets
         try:
             # Sky subset does not have area. Not worth it to calculate just for a warning.
             if hasattr(self.aperture.selected_spatial_region, 'area'):
                 self.aperture_area = int(np.ceil(self.aperture.selected_spatial_region.area))
@@ -261,30 +294,48 @@
         except Exception as e:
             self.hub.broadcast(SnackbarMessage(
                 f"Failed to extract {self.aperture_selected}: {repr(e)}",
                 color='error', sender=self))
         else:
             self._background_selected_changed()
 
+    @property
+    def _cubeviz_slice_ind(self):
+        fv = self.app.get_viewer(self.app._jdaviz_helper._default_flux_viewer_reference_name)
+        return fv.slice
+
     def _calc_background_median(self, reg, data=None):
         # Basically same way image stats are calculated in vue_do_aper_phot()
         # except here we only care about one stat for the background.
         if data is None:
             if self.multiselect:
                 if len(self.dataset.selected) == 1:
                     data = self.dataset.selected_dc_item[0]
                 else:
                     raise ValueError("cannot calculate background median in multiselect")
             else:
                 data = self.dataset.selected_dc_item
+
         comp = data.get_component(data.main_components[0])
+
+        if self.config == "cubeviz" and data.ndim > 2:
+            comp_data = comp.data[:, :, self._cubeviz_slice_ind].T  # nx, ny --> ny, nx
+            # Similar to coords_info logic.
+            if '_orig_spec' in getattr(data, 'meta', {}):
+                w = data.meta['_orig_spec'].wcs.celestial
+            else:
+                w = data.coords.celestial
+        else:  # "imviz"
+            comp_data = comp.data  # ny, nx
+            w = data.coords
+
         if hasattr(reg, 'to_pixel'):
-            reg = reg.to_pixel(data.coords)
+            reg = reg.to_pixel(w)
         aper_mask_stat = reg.to_mask(mode='center')
-        img_stat = aper_mask_stat.get_values(comp.data, mask=None)
+        img_stat = aper_mask_stat.get_values(comp_data, mask=None)
 
         # photutils/background/_utils.py --> nanmedian()
         return np.nanmedian(img_stat)  # Naturally in data unit
 
     @observe('background_selected')
     def _background_selected_changed(self, event={}):
         background_selected = event.get('new', self.background_selected)
@@ -345,21 +396,29 @@
             if dataset not in self.dataset.choices:  # pragma: no cover
                 raise ValueError(f"dataset must be one of {self.dataset.choices}")
             data = self.dataset._get_dc_item(dataset)
         else:
             # we can use the pre-cached value
             data = self.dataset.selected_dc_item
 
-        if aperture is not None and aperture not in self.aperture.choices:
-            raise ValueError(f"aperture must be one of {self.aperture.choices}")
+        if aperture is not None:
+            if aperture not in self.aperture.choices:
+                raise ValueError(f"aperture must be one of {self.aperture.choices}")
+
         if aperture is not None or dataset is not None:
             reg = self.aperture._get_spatial_region(subset=aperture if aperture is not None else self.aperture.selected,  # noqa
                                                     dataset=dataset if dataset is not None else self.dataset.selected)  # noqa
+            # determine if a valid aperture (since selected_validity only applies to selected entry)
+            _, _, validity = self.aperture._get_mark_coords_and_validate(selected=aperture)
+            if not validity.get('is_aperture'):
+                raise ValueError(f"Selected aperture {aperture} is not valid: {validity.get('aperture_message')}")  # noqa
         else:
             # use the pre-cached value
+            if not self.aperture.selected_validity.get('is_aperture'):
+                raise ValueError(f"Selected aperture is not valid: {self.aperture.selected_validity.get('aperture_message')}")  # noqa
             reg = self.aperture.selected_spatial_region
 
         # Reset last fitted model
         fit_model = None
         # TODO: remove _fitted_model_name cache?
         if self._fitted_model_name in self.app.fitted_models:
             del self.app.fitted_models[self._fitted_model_name]
@@ -383,30 +442,46 @@
                                                        dataset=dataset if dataset is not None else self.dataset.selected)  # noqa
             background_value = self._calc_background_median(bg_reg, data=data)
         try:
             bg = float(background_value)
         except ValueError:  # Clearer error message
             raise ValueError('Missing or invalid background value')
 
+        if self.config == "cubeviz" and data.ndim > 2:
+            comp_data = comp.data[:, :, self._cubeviz_slice_ind].T  # nx, ny --> ny, nx
+            # Similar to coords_info logic.
+            if '_orig_spec' in getattr(data, 'meta', {}):
+                w = data.meta['_orig_spec'].wcs
+            else:
+                w = data.coords
+        else:  # "imviz"
+            comp_data = comp.data  # ny, nx
+            w = data.coords
+
         if hasattr(reg, 'to_pixel'):
             sky_center = reg.center
-            xcenter, ycenter = data.coords.world_to_pixel(sky_center)
+            if self.config == "cubeviz" and data.ndim > 2:
+                ycenter, xcenter = w.world_to_pixel(self._cube_wave, sky_center)[1]
+            else:  # "imviz"
+                xcenter, ycenter = w.world_to_pixel(sky_center)
         else:
             xcenter = reg.center.x
             ycenter = reg.center.y
             if data.coords is not None:
-                sky_center = data.coords.pixel_to_world(xcenter, ycenter)
+                if self.config == "cubeviz" and data.ndim > 2:
+                    sky_center = w.pixel_to_world(self._cubeviz_slice_ind, ycenter, xcenter)[1]
+                else:  # "imviz"
+                    sky_center = w.pixel_to_world(xcenter, ycenter)
             else:
                 sky_center = None
 
         aperture = regions2aperture(reg)
         include_pixarea_fac = False
         include_counts_fac = False
         include_flux_scale = False
-        comp_data = comp.data
         if comp.units:
             img_unit = u.Unit(comp.units)
             bg = bg * img_unit
             comp_data = comp_data << img_unit
 
             if u.sr in img_unit.bases:  # TODO: Better way to detect surface brightness unit?
                 try:
@@ -467,14 +542,21 @@
              reg.meta.get('label', ''), Time(datetime.now(tz=timezone.utc))],
             names=['xcenter', 'ycenter', 'sky_center', 'background', 'pixarea_tot',
                    'aperture_sum_counts', 'aperture_sum_counts_err', 'counts_fac',
                    'aperture_sum_mag', 'flux_scaling',
                    'data_label', 'subset_label', 'timestamp'],
             indexes=[1, 1, 1, 1, 3, 3, 3, 3, 3, 3, 18, 18, 18])
 
+        if self.config == "cubeviz":
+            if data.ndim > 2:
+                slice_val = self._cube_wave
+            else:
+                slice_val = u.Quantity(np.nan, self._cube_wave.unit)
+            phot_table.add_column(slice_val, name="slice_wave", index=29)
+
         if add_to_table:
             try:
                 phot_table['id'][0] = self.table._qtable['id'].max() + 1
                 self.table.add_item(phot_table)
             except Exception:  # Discard incompatible QTable
                 self.table.clear_table()
                 phot_table['id'][0] = 1
@@ -482,38 +564,47 @@
 
             # User wants 'sum' as scientific notation.
             self.table._qtable['sum'].info.format = '.6e'
 
         # Plots.
         if update_plots:
             if self.current_plot_type == "Curve of Growth":
-                self.plot.figure.title = 'Curve of growth from aperture center'
+                if self.config == "cubeviz" and data.ndim > 2:
+                    self.plot.figure.title = f'Curve of growth from aperture center at {slice_val:.4e}'  # noqa: E501
+                else:
+                    self.plot.figure.title = 'Curve of growth from aperture center'
                 x_arr, sum_arr, x_label, y_label = _curve_of_growth(
                     comp_data, (xcenter, ycenter), aperture, phot_table['sum'][0],
                     wcs=data.coords, background=bg, pixarea_fac=pixarea_fac)
                 self.plot._update_data('profile', x=x_arr, y=sum_arr, reset_lims=True)
                 self.plot.update_style('profile', line_visible=True, color='gray', size=32)
                 self.plot.update_style('fit', visible=False)
                 self.plot.figure.axes[0].label = x_label
                 self.plot.figure.axes[1].label = y_label
 
             else:  # Radial profile
                 self.plot.figure.axes[0].label = 'pix'
                 self.plot.figure.axes[1].label = comp.units or 'Value'
 
                 if self.current_plot_type == "Radial Profile":
-                    self.plot.figure.title = 'Radial profile from aperture center'
+                    if self.config == "cubeviz" and data.ndim > 2:
+                        self.plot.figure.title = f'Radial profile from aperture center at {slice_val:.4e}'  # noqa: E501
+                    else:
+                        self.plot.figure.title = 'Radial profile from aperture center'
                     x_data, y_data = _radial_profile(
                         phot_aperstats.data_cutout, phot_aperstats.bbox, (xcenter, ycenter),
                         raw=False)
                     self.plot._update_data('profile', x=x_data, y=y_data, reset_lims=True)
                     self.plot.update_style('profile', line_visible=True, color='gray', size=32)
 
                 else:  # Radial Profile (Raw)
-                    self.plot.figure.title = 'Raw radial profile from aperture center'
+                    if self.config == "cubeviz" and data.ndim > 2:
+                        self.plot.figure.title = f'Raw radial profile from aperture center at {slice_val:.4e}'  # noqa: E501
+                    else:
+                        self.plot.figure.title = 'Raw radial profile from aperture center'
                     x_data, y_data = _radial_profile(
                         phot_aperstats.data_cutout, phot_aperstats.bbox, (xcenter, ycenter),
                         raw=True)
 
                     self.plot._update_data('profile', x=x_data, y=y_data, reset_lims=True)
                     self.plot.update_style('profile', line_visible=False, color='gray', size=10)
 
@@ -552,53 +643,32 @@
         for key in phot_table.colnames:
             if key in ('id', 'data_label', 'subset_label', 'background', 'pixarea_tot',
                        'counts_fac', 'aperture_sum_counts_err', 'flux_scaling', 'timestamp'):
                 continue
             x = phot_table[key][0]
             if (isinstance(x, (int, float, u.Quantity)) and
                     key not in ('xcenter', 'ycenter', 'sky_center', 'sum_aper_area',
-                                'aperture_sum_counts', 'aperture_sum_mag')):
+                                'aperture_sum_counts', 'aperture_sum_mag', 'slice_wave')):
                 tmp.append({'function': key, 'result': f'{x:.4e}'})
             elif key == 'sky_center' and x is not None:
                 tmp.append({'function': 'RA center', 'result': f'{x.ra.deg:.6f} deg'})
                 tmp.append({'function': 'Dec center', 'result': f'{x.dec.deg:.6f} deg'})
             elif key in ('xcenter', 'ycenter', 'sum_aper_area'):
                 tmp.append({'function': key, 'result': f'{x:.1f}'})
             elif key == 'aperture_sum_counts' and x is not None:
                 tmp.append({'function': key, 'result':
                             f'{x:.4e} ({phot_table["aperture_sum_counts_err"][0]:.4e})'})
             elif key == 'aperture_sum_mag' and x is not None:
                 tmp.append({'function': key, 'result': f'{x:.3f}'})
+            elif key == 'slice_wave':
+                if data.ndim > 2:
+                    tmp.append({'function': key, 'result': f'{slice_val:.4e}'})
             else:
                 tmp.append({'function': key, 'result': str(x)})
 
-            # Parse results for GUI.
-            tmp = []
-            for key in phot_table.colnames:
-                if key in ('id', 'data_label', 'subset_label', 'background', 'pixarea_tot',
-                           'counts_fac', 'aperture_sum_counts_err', 'flux_scaling', 'timestamp'):
-                    continue
-                x = phot_table[key][0]
-                if (isinstance(x, (int, float, u.Quantity)) and
-                        key not in ('xcenter', 'ycenter', 'sky_center', 'sum_aper_area',
-                                    'aperture_sum_counts', 'aperture_sum_mag')):
-                    tmp.append({'function': key, 'result': f'{x:.4e}'})
-                elif key == 'sky_center' and x is not None:
-                    tmp.append({'function': 'RA center', 'result': f'{x.ra.deg:.6f} deg'})
-                    tmp.append({'function': 'Dec center', 'result': f'{x.dec.deg:.6f} deg'})
-                elif key in ('xcenter', 'ycenter', 'sum_aper_area'):
-                    tmp.append({'function': key, 'result': f'{x:.1f}'})
-                elif key == 'aperture_sum_counts' and x is not None:
-                    tmp.append({'function': key, 'result':
-                                f'{x:.4e} ({phot_table["aperture_sum_counts_err"][0]:.4e})'})
-                elif key == 'aperture_sum_mag' and x is not None:
-                    tmp.append({'function': key, 'result': f'{x:.3f}'})
-                else:
-                    tmp.append({'function': key, 'result': str(x)})
-
         if update_plots:
             # Also display fit results
             fit_tmp = []
             if fit_model is not None and isinstance(fit_model, Gaussian1D):
                 for param in ('mean', 'fwhm', 'amplitude'):
                     p_val = getattr(fit_model, param)
                     if isinstance(p_val, Parameter):
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.vue` & `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.vue`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,63 @@
 <template>
   <j-tray-plugin
-    description='Perform aperture photometry for drawn regions.'
+    :description="docs_description || 'Perform aperture photometry for drawn regions.'"
     :link="docs_link || 'https://jdaviz.readthedocs.io/en/'+vdocs+'/'+config+'/plugins.html#simple-aperture-photometry'"
-    :popout_button="popout_button">
-
-    <v-row>
-      <div style="width: calc(100% - 32px)">
-      </div>
-      <div style="width: 32px">
-        <j-tooltip tooltipcontent="Toggle batch mode">
-          <v-btn
-            icon
-            style="opacity: 0.7"
-            @click="() => {multiselect = !multiselect}"
-          >
-            <img :src="multiselect ? icon_checktoradial : icon_radialtocheck" width="24" class="invert-if-dark"/>
-          </v-btn>
-        </j-tooltip>
-      </div>
-    </v-row>
+    :uses_active_status="uses_active_status"
+    @plugin-ping="plugin_ping($event)"
+    :keep_active.sync="keep_active"
+    :popout_button="popout_button"
+    :scroll_to.sync="scroll_to">
+
+    <j-multiselect-toggle
+      :multiselect.sync="multiselect"
+      :icon_checktoradial="icon_checktoradial"
+      :icon_radialtocheck="icon_radialtocheck"
+      tooltip="Toggle batch mode"
+    ></j-multiselect-toggle>
 
     <plugin-dataset-select
       :items="dataset_items"
       :selected.sync="dataset_selected"
       :multiselect="multiselect"
       :show_if_single_entry="false"
       label="Data"
       hint="Select the data for photometry."
     />
 
+    <div v-if='config == "cubeviz" && is_cube'>
+      <v-row class="row-no-outside-padding row-min-bottom-padding">
+        <v-col>
+          <v-text-field
+            :value="cube_slice"
+            class="mt-0 pt-0"
+            label="Slice wavelength"
+            hint="Extracts photometry from currently selected cube slice"
+            disabled
+          ></v-text-field>
+        </v-col>
+      </v-row>
+    </div>
+
     <div v-if='dataset_selected.length > 0'>
       <plugin-subset-select
         :items="aperture_items"
         :selected.sync="aperture_selected"
         :multiselect="multiselect"
         :show_if_single_entry="true"
         label="Aperture"
         hint="Select aperture region for photometry (cannot be an annulus or composite subset)."
       />
 
+      <v-row v-if="aperture_selected.length && !aperture_selected_validity.is_aperture">
+        <span class="v-messages v-messages__message text--secondary" style="color: red !important">
+            {{aperture_selected}} is not a valid aperture: {{aperture_selected_validity.aperture_message}}.
+        </span>
+      </v-row>
+
       <div v-if="aperture_selected.length > 0">
         <plugin-subset-select
           :items="background_items"
           :selected.sync="background_selected"
           :show_if_single_entry="true"
           label="Background"
           hint="Select subset region for background calculation (cannot be a composite subset)."
@@ -154,15 +169,15 @@
         </v-row>
 
         <v-row justify="end">
           <plugin-action-button
             :results_isolated_to_plugin="true"
             @click="do_aper_phot"
             :spinner="spinner"
-            :disabled="aperture_selected === background_selected"
+            :disabled="aperture_selected === background_selected || !aperture_selected_validity.is_aperture"
           >
             Calculate
           </plugin-action-button>
         </v-row>
       </div>
     </div>
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/plugins/catalogs/catalogs.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/catalogs/catalogs.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,18 +54,28 @@
 
         if 'sky_centroid' not in table.colnames:
             return 'Table does not contain required sky_centroid column', {}
 
         return '', {path: table}
 
     @with_spinner()
-    def search(self):
-        """
-        Search the catalog, display markers on the viewer, and return a table of results (or None
-        if no results available)
+    def search(self, error_on_fail=False):
+        """Search the catalog, display markers on the viewer, and return results if available.
+
+        Parameters
+        ----------
+        error_on_fail : bool
+            Throw exception when query fails instead of a red snackbar message.
+            This is useful for debugging.
+
+        Returns
+        -------
+        skycoord_table : `~astropy.coordinates.SkyCoord` or `None`
+            Sky coordinates (or None if no results available).
+
         """
         # calling clear in the case the user forgot after searching
         self.clear()
 
         # gets the current viewer
         viewer = self.viewer.selected_obj
 
@@ -107,17 +117,19 @@
                         f"Radius for {self.catalog_selected} has max radius of {r_max} but got "
                         f"{zoom_radius.to(u.arcmin)}, using {r_max}.",
                         color='warning', sender=self))
                     zoom_radius = r_max
                 query_region_result = SDSS.query_region(skycoord_center, radius=zoom_radius,
                                                         data_release=17)
             except Exception as e:  # nosec
-                self.hub.broadcast(SnackbarMessage(
-                    f"Failed to query {self.catalog_selected} with c={skycoord_center} and "
-                    f"r={zoom_radius}: {repr(e)}", color='error', sender=self))
+                errmsg = (f"Failed to query {self.catalog_selected} with c={skycoord_center} and "
+                          f"r={zoom_radius}: {repr(e)}")
+                if error_on_fail:
+                    raise Exception(errmsg) from e
+                self.hub.broadcast(SnackbarMessage(errmsg, color='error', sender=self))
                 query_region_result = None
 
             if query_region_result is None:
                 self.results_available = True
                 self.number_of_results = 0
                 self.app._catalog_source_table = None
                 viewer.remove_markers(marker_name=self._marker_name)
@@ -204,15 +216,15 @@
             self.results_available = False
             self.number_of_results = 0
 
             # all markers are removed from the viewer
             viewer.remove_markers(marker_name=self._marker_name)
 
         elif self.results_available:
-            from jdaviz.configs.imviz.helper import layer_is_table_data
+            from jdaviz.utils import layer_is_table_data
 
             # resetting values
             self.results_available = False
             self.number_of_results = 0
 
             # markers still there, just hidden
             for lyr in viewer.layers:
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/plugins/catalogs/catalogs.vue` & `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/catalogs/catalogs.vue`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 <template>
   <j-tray-plugin
-     description='Queries an area encompassed by the viewer using a specified catalog and marks all the objects found within the area.'
+    :description="docs_description || 'Queries an area encompassed by the viewer using a specified catalog and marks all the objects found within the area.'"
     :link="docs_link || 'https://jdaviz.readthedocs.io/en/'+vdocs+'/'+config+'/plugins.html#catalog-search'"
-    :popout_button="popout_button">
+    :popout_button="popout_button"
+    :scroll_to.sync="scroll_to">
 
     <plugin-viewer-select
        :items="viewer_items"
        :selected.sync="viewer_selected"
        label="Viewer"
        :show_if_single_entry="false"
        hint="Select a viewer to search."
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/plugins/compass/compass.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/compass/compass.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/plugins/compass/compass.vue` & `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/compass/compass.vue`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 <template>
   <j-tray-plugin
-    description='Show active data label, compass, and zoom box.'
+    :description="docs_description || 'Show active data label, compass, and zoom box.'"
     :link="docs_link || 'https://jdaviz.readthedocs.io/en/'+vdocs+'/'+config+'/plugins.html#compass'"
     :uses_active_status="uses_active_status"
     @plugin-ping="plugin_ping($event)"
-    :popout_button="popout_button">
+    :popout_button="popout_button"
+    :scroll_to.sync="scroll_to">
 
     <plugin-viewer-select
       :items="viewer_items"
       :selected.sync="viewer_selected"
       label="Viewer"
       hint="Select a viewer to show."
     />
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/plugins/coords_info/coords_info.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/coords_info/coords_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         viewer_refs = []
         for viewer in self.app._viewer_store.values():
             if isinstance(viewer, self._supported_viewer_classes):
                 self._create_viewer_callbacks(viewer)
                 viewer_refs.append(viewer.reference_id)
 
         self.dataset._manual_options = ['auto', 'none']
-        self.dataset.filters = ['layer_in_viewers']
+        self.dataset.filters = ['layer_in_viewers', 'is_not_wcs_only']
         if self.app.config == 'imviz':
             # filter out scatter-plot entries (from add_markers API, for example)
             self.dataset.add_filter('is_image')
         # we also want to include auto-collapsed spectra (spatial subsets)
         self.dataset._cubeviz_include_spatial_subsets()
 
         # subscribe to mouse events on any new viewers
@@ -222,14 +222,33 @@
         self._dict = {}
         if isinstance(viewer, SpecvizProfileView):
             self._spectrum_viewer_update(viewer, x, y)
         elif isinstance(viewer,
                         (ImvizImageView, CubevizImageView, MosvizImageView, MosvizProfile2DView)):
             self._image_viewer_update(viewer, x, y)
 
+    def _image_shape_inds(self, image):
+        # return the indices in image.shape for the x and y dimension, respectively
+        if image.ndim == 3:
+            # cubeviz case
+            return (0, 1)  # (ix_shape, iy_shape)
+        elif image.ndim == 2:
+            return (1, 0)  # (ix_shape, iy_shape)
+        else:  # pragma: no cover
+            raise ValueError(f'does not support ndim={image.ndim}')
+
+    def _get_cube_value(self, image, arr, x, y, viewer):
+        if image.ndim == 3:
+            # cubeviz case:
+            return arr[int(round(x)), int(round(y)), viewer.state.slices[-1]]
+        elif image.ndim == 2:
+            return arr[int(round(y)), int(round(x))]
+        else:  # pragma: no cover
+            raise ValueError(f'does not support ndim={image.ndim}')
+
     def _image_viewer_update(self, viewer, x, y):
         # Display the current cursor coordinates (both pixel and world) as
         # well as data values. For now we use the first dataset in the
         # viewer for the data values.
 
         # Extract first dataset from visible layers and use this for coordinates - the choice
         # of dataset shouldn't matter if the datasets are linked correctly
@@ -304,31 +323,31 @@
                 wcs_ndim = coo_data.ndim
             else:
                 data_wcs = None
 
             if data_wcs:
                 try:
                     if wcs_ndim == 3:
-                        sky = data_wcs.pixel_to_world(viewer.state.slices[-1], y, x)[1].icrs
+                        sky = data_wcs.pixel_to_world(viewer.slice, y, x)[1].icrs
                     else:  # wcs_ndim == 2
                         sky = data_wcs.pixel_to_world(x, y).icrs
                 except Exception:
                     coords_status = False
                 else:
                     coords_status = True
             else:
                 self.reset_coords_display()
                 coords_status = False
 
             slice_plugin = self.app._jdaviz_helper.plugins.get('Slice', None)
             if slice_plugin is not None and len(image.shape) == 3:
                 # float to be compatible with default value of nan
-                self._dict['slice'] = float(slice_plugin.slice)
-                self._dict['spectral_axis'] = slice_plugin.wavelength
-                self._dict['spectral_axis:unit'] = slice_plugin._obj.wavelength_unit
+                self._dict['slice'] = float(viewer.slice)
+                self._dict['spectral_axis'] = slice_plugin.value
+                self._dict['spectral_axis:unit'] = slice_plugin._obj.value_unit
 
         elif isinstance(viewer, MosvizImageView):
 
             if data_has_valid_wcs(image, ndim=2):
                 try:
                     sky = image.coords.pixel_to_world(x, y).icrs
                 except Exception:  # WCS might not be celestial  # pragma: no cover
@@ -402,37 +421,26 @@
             # no data values to extract
             self.row1b_title = ''
             self.row1b_text = ''
             return
 
         # Extract data values at this position.
         # Check if shape is [x, y, z] or [y, x] and show value accordingly.
-        if image.ndim == 3:
-            # needed for cubeviz
-            ix_shape = 0
-            iy_shape = 1
-        elif image.ndim == 2:
-            ix_shape = 1
-            iy_shape = 0
-        else:  # pragma: no cover
-            raise ValueError(f'does not support ndim={image.ndim}')
+        ix_shape, iy_shape = self._image_shape_inds(image)
 
         if (-0.5 < x < image.shape[ix_shape] - 0.5 and -0.5 < y < image.shape[iy_shape] - 0.5
                 and hasattr(active_layer, 'attribute')):
             attribute = active_layer.attribute
             if isinstance(viewer, (ImvizImageView, MosvizImageView, MosvizProfile2DView)):
                 value = image.get_data(attribute)[int(round(y)), int(round(x))]
                 unit = image.get_component(attribute).units
             elif isinstance(viewer, CubevizImageView):
                 arr = image.get_component(attribute).data
                 unit = image.get_component(attribute).units
-                if image.ndim == 3:
-                    value = arr[int(round(x)), int(round(y)), viewer.state.slices[-1]]
-                else:  # 2
-                    value = arr[int(round(y)), int(round(x))]
+                value = self._get_cube_value(image, arr, x, y, viewer)
             self.row1b_title = 'Value'
             self.row1b_text = f'{value:+10.5e} {unit}'
             self._dict['value'] = float(value)
             self._dict['value:unit'] = unit
             self._dict['value:unreliable'] = unreliable_pixel
         else:
             self.row1b_title = ''
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/plugins/coords_info/coords_info.vue` & `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/coords_info/coords_info.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/plugins/footprints/footprints.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/footprints/footprints.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from traitlets import Bool, List, Unicode, observe
 import numpy as np
 import regions
 
 from glue.core.message import DataCollectionAddMessage, DataCollectionDeleteMessage
 
 from jdaviz.core.custom_traitlets import FloatHandleEmpty
-from jdaviz.core.events import LinkUpdatedMessage
+from jdaviz.core.events import LinkUpdatedMessage, ChangeRefDataMessage
 from jdaviz.core.marks import FootprintOverlay
 from jdaviz.core.region_translators import regions2roi
 from jdaviz.core.registries import tray_registry
 from jdaviz.core.template_mixin import (PluginTemplateMixin, ViewerSelectMixin,
                                         EditableSelectPluginComponent,
                                         FileImportSelectPluginComponent, HasFileImportSelect)
 from jdaviz.core.user_api import PluginUserApi
@@ -127,14 +127,15 @@
         # set the custom file parser for importing catalogs
         self.preset._file_parser = self._file_parser
 
         # disable if pixel-linked AND only a single item in the data collection
         self.hub.subscribe(self, LinkUpdatedMessage, handler=self._on_link_type_updated)
         self.hub.subscribe(self, DataCollectionAddMessage, handler=self._on_link_type_updated)
         self.hub.subscribe(self, DataCollectionDeleteMessage, handler=self._on_link_type_updated)
+        self.hub.subscribe(self, ChangeRefDataMessage, handler=lambda _: self._preset_args_changed())  # noqa
         self._on_link_type_updated()
 
     @property
     def user_api(self):
         return PluginUserApi(self, expose=('overlay',
                                            'rename_overlay', 'add_overlay', 'remove_overlay',
                                            'viewer', 'visible', 'color', 'fill_opacity',
@@ -184,15 +185,15 @@
         # toggle visibility as necessary
         self._on_is_active_changed()
 
     def vue_link_by_wcs(self, *args):
         # call other plugin so that other options (wcs_use_affine, wcs_use_fallback)
         # are retained.  Remove this method if support for plotting footprints
         # when pixel-linked is reintroduced.
-        self.app._jdaviz_helper.plugins['Links Control'].link_type = 'WCS'
+        self.app._jdaviz_helper.plugins['Orientation'].link_type = 'WCS'
 
     def _ensure_first_overlay(self):
         if not len(self._overlays):
             # create the first default overlay
             self._change_overlay()
             # update the marks
             self._preset_args_changed()
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/plugins/footprints/footprints.vue` & `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/footprints/footprints.vue`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 <template>
   <j-tray-plugin
-    description='Show instrument footprints as overlays on image viewers.'
+    :description="docs_description || 'Show instrument footprints as overlays on image viewers.'"
     :link="docs_link || 'https://jdaviz.readthedocs.io/en/'+vdocs+'/'+config+'/plugins.html#footprints'"
     :uses_active_status="uses_active_status"
     @plugin-ping="plugin_ping($event)"
     :keep_active.sync="keep_active"
     :disabled_msg="disabled_msg"
-    :popout_button="popout_button">
+    :popout_button="popout_button"
+    :scroll_to.sync="scroll_to">
 
     <plugin-editable-select
       :mode.sync="overlay_mode"
       :edit_value.sync="overlay_edit_value"
       :items="overlay_items"
       :selected.sync="overlay_selected"
       label="Overlay"
       hint="Select an overlay to modify."
       >
     </plugin-editable-select>
 
-    <div v-if="is_pixel_linked">
-      <v-alert type='warning' style="margin-left: -12px; margin-right: -12px">
-          cannot plot footprint when pixel-linked (see Links Control plugin)
-          <v-row justify="center">
-            <v-btn @click="link_by_wcs">
-              link by WCS
-            </v-btn>
-          </v-row>
-      </v-alert>
-    </div>
-    <div v-if="viewer_items.length===0">
-      <v-alert type='warning' style="margin-left: -12px; margin-right: -12px">
-          no valid viewers (with necessary WCS information) to show footprint overlay
-      </v-alert>
-    </div>
+    <v-alert v-if="is_pixel_linked" type='warning' style="margin-left: -12px; margin-right: -12px">
+      cannot plot footprint when aligned by pixels (see Orientation plugin).
+      <v-row justify="end" style="margin-right: 2px; margin-top: 16px">
+        <v-btn @click="link_by_wcs">
+          link by WCS
+        </v-btn>
+      </v-row>
+    </v-alert>
+    <v-alert v-if="viewer_items.length===0" type='warning' style="margin-left: -12px; margin-right: -12px">
+      no valid viewers (with necessary WCS information) to show footprint overlay.
+    </v-alert>
   
     <div v-if="!is_pixel_linked && viewer_items.length > 0 && overlay_selected.length > 0">
       <j-plugin-section-header>Display Options</j-plugin-section-header>
 
       <plugin-viewer-select
         :items="viewer_items"
         :selected.sync="viewer_selected"
@@ -75,15 +72,15 @@
       <div>
         <v-subheader class="pl-0 slider-label" style="height: 12px">Fill Opacity</v-subheader>
         <glue-throttled-slider wait="300" max="1" step="0.01" :value.sync="fill_opacity" hide-details class="no-hint" />
       </div>
 
       <j-plugin-section-header>Footprint Definition</j-plugin-section-header>
       <v-alert v-if="!has_pysiaf" type="warning" style="margin-left: -12px; margin-right: -12px">
-        <span>To use JWST footprints, install pysiaf and restart jdaviz</span>
+        To use JWST footprints, install pysiaf and restart jdaviz.
       </v-alert>
 
       <plugin-file-import-select
         :items="preset_items"
         :selected.sync="preset_selected"
         label="Preset"
         hint="Preset instrument or import from a file."
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/plugins/footprints/preset_regions.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/footprints/preset_regions.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,154 +1,137 @@
-import numpy as np
+import os
 from traitlets import Bool, Unicode, observe
 
-from jdaviz.configs.imviz.helper import get_top_layer_index
+from glue_jupyter.common.toolbar_vuetify import read_icon
+
+from jdaviz.configs.imviz.wcs_utils import get_compass_info
 from jdaviz.core.custom_traitlets import FloatHandleEmpty
-from jdaviz.core.events import ViewerAddedMessage
+from jdaviz.core.events import AddDataMessage, RemoveDataMessage, CanvasRotationChangedMessage
 from jdaviz.core.registries import tray_registry
-from jdaviz.core.template_mixin import (PluginTemplateMixin, ViewerSelectMixin, Plot,
-                                        skip_if_no_updates_since_last_active)
-
-__all__ = ['LineProfileXY']
-
-
-@tray_registry('imviz-line-profile-xy', label="Imviz Line Profiles (XY)")
-class LineProfileXY(PluginTemplateMixin, ViewerSelectMixin):
-    template_file = __file__, "line_profile_xy.vue"
-    uses_active_status = Bool(True).tag(sync=True)
-
-    plot_available = Bool(False).tag(sync=True)
-    selected_x = FloatHandleEmpty('').tag(sync=True)
-    selected_y = FloatHandleEmpty('').tag(sync=True)
+from jdaviz.core.template_mixin import PluginTemplateMixin, ViewerSelectMixin
+from jdaviz.core.user_api import PluginUserApi
+from jdaviz.core.tools import ICON_DIR
+
+__all__ = ['RotateCanvas']
+
+
+@tray_registry('imviz-rotate-canvas', label="Canvas Rotation", viewer_requirements='image')
+class RotateCanvas(PluginTemplateMixin, ViewerSelectMixin):
+    """
+    See the :ref:`Canvas Rotation Plugin Documentation <rotate-canvas>` for more details.
+
+    Only the following attributes and methods are available through the
+    :ref:`public plugin API <plugin-apis>`:
+
+    * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.show`
+    * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.open_in_tray`
+    * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.close_in_tray`
+    * ``viewer`` (:class:`~jdaviz.core.template_mixin.ViewerSelect`):
+      Viewer to show orientation/compass information.
+    * ``angle``:
+      Angle to rotate the axes canvas, clockwise.
+    * ``flip_horizontal``:
+      Whether to flip the canvas horizontally, after applying rotation.
+    * :meth:`reset`
+    * :meth:`set_north_up_east_left`
+    * :meth:`set_north_up_east_right`
+    """
+    template_file = __file__, "rotate_canvas.vue"
+
+    angle = FloatHandleEmpty(0).tag(sync=True)  # degrees, clockwise
+    flip_horizontal = Bool(False).tag(sync=True)  # horizontal flip applied after rotation
+    has_wcs = Bool(False).tag(sync=True)
 
-    plot_across_x_widget = Unicode().tag(sync=True)
-    plot_across_y_widget = Unicode().tag(sync=True)
+    icon_nuer = Unicode(read_icon(os.path.join(ICON_DIR, 'right-east.svg'), 'svg+xml')).tag(sync=True)  # noqa
+    icon_nuel = Unicode(read_icon(os.path.join(ICON_DIR, 'left-east.svg'), 'svg+xml')).tag(sync=True)  # noqa
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-        self.plot_across_x = Plot(self)
-        self.plot_across_y = Plot(self)
-        for plot in (self.plot_across_x, self.plot_across_y):
-            # override default styling
-            plot.figure.fig_margin = {'top': 60, 'bottom': 60, 'left': 65, 'right': 15}
-            plot.viewer.axis_x.num_ticks = 5
-            plot.viewer.axis_y.tick_format = '0.2e'
-            plot.viewer.axis_y.label_offset = '55px'
-
-        self.plot_across_x_widget = 'IPY_MODEL_'+self.plot_across_x.model_id
-        self.plot_across_y_widget = 'IPY_MODEL_'+self.plot_across_y.model_id
-
-        self.hub.subscribe(self, ViewerAddedMessage, handler=self._on_viewer_added)
-
-    def reset_results(self):
-        self.plot_available = False
-        self.plot_across_x.update_style('line', visible=False)
-        self.plot_across_x.clear_all_marks()
-        self.plot_across_y.clear_all_marks()
+        self.hub.subscribe(self, AddDataMessage, handler=self._on_viewer_data_changed)
+        self.hub.subscribe(self, RemoveDataMessage, handler=self._on_viewer_data_changed)
 
-    def _create_viewer_callbacks(self, viewer):
-        if not self.is_active:
-            return
-
-        callback = self._viewer_callback(viewer, self._on_viewer_key_event)
-        viewer.add_event_callback(callback, events=['keydown'])
-
-    def _on_viewer_added(self, msg):
-        self._create_viewer_callbacks(self.app.get_viewer_by_id(msg.viewer_id))
+    @property
+    def user_api(self):
+        return PluginUserApi(self, expose=('viewer', 'angle', 'flip_horizontal', 'reset',
+                                           'set_north_up_east_right', 'set_north_up_east_left'))
+
+    @property
+    def ref_data(self):
+        return self.app.get_viewer_by_id(self.viewer.selected_id).state.reference_data
 
-    @observe('is_active')
-    def _is_active_changed(self, msg):
-        # subscribe/unsubscribe to keypress events across all viewers
-        for viewer in self.app._viewer_store.values():
-            if not hasattr(viewer, 'figure'):
-                # table viewer, etc
-                continue
-            callback = self._viewer_callback(viewer, self._on_viewer_key_event)
-
-            if self.is_active:
-                viewer.add_event_callback(callback, events=['keydown'])
-            else:
-                viewer.remove_event_callback(callback)
-
-        # pass along the msg object so that @skip_if_no_updates_since_last_active can be used
-        # to avoid re-drawing if no changes since the last time is_active was set
-        self.vue_draw_plot(msg)
-
-    def _on_viewer_key_event(self, viewer, data):
-        if data['key'] == 'l':
-            image = viewer.active_image_layer.layer
-            x = data['domain']['x']
-            y = data['domain']['y']
-            if x is None or y is None:  # Out of bounds
-                return
-            x, y, _, _ = viewer._get_real_xy(image, x, y)
-            self.selected_x = x
-            self.selected_y = y
-            self.viewer_selected = viewer.reference_id
-            # TODO: remove manual calls to vue_draw_plot and trigger
-            # by changes to selected_x/selected_y as well as viewer_selected
-            self.vue_draw_plot()
-
-    @observe("viewer_selected")
-    @skip_if_no_updates_since_last_active()  # called with msg passed along from _is_active_changed
-    def vue_draw_plot(self, msg={}):
-        """Draw line profile plots for given Data across given X and Y indices (0-indexed)."""
-        if not self.selected_x or not self.selected_y:
+    def _on_viewer_data_changed(self, msg=None):
+        if not self.viewer_selected:  # pragma: no cover
             return
+        self.has_wcs = getattr(self.ref_data, 'coords', None) is not None
 
-        viewer = self.viewer.selected_obj
-        i = get_top_layer_index(viewer)
-        data = viewer.state.layers[i].layer
-
-        x = int(round(self.selected_x))
-        y = int(round(self.selected_y))
-
-        nx = data.shape[1]
-        ny = data.shape[0]
-        if x < 0 or y < 0 or x >= nx or y >= ny:
-            self.reset_results()
+    @observe('viewer_selected')
+    def _viewer_selected_changed(self, *args, **kwargs):
+        if not hasattr(self, 'viewer'):
             return
-
-        comp = data.get_component(data.main_components[0])
-        if comp.units:
-            y_label = comp.units
-        else:
-            y_label = 'Value'
-
-        xy_limits = viewer._get_zoom_limits(data)
-        x_limits = xy_limits[:, 0]
-        y_limits = xy_limits[:, 1]
-        x_min = max(int(x_limits.min()), 0)
-        x_max = min(int(x_limits.max()), nx)
-        y_min = max(int(y_limits.min()), 0)
-        y_max = min(int(y_limits.max()), ny)
-
-        self.plot_across_x.figure.title = f'X={x}'
-        self.plot_across_x._update_data('line', x=range(comp.data.shape[0]), y=comp.data[:, x],
-                                        reset_lims=False)
-        zoomed_data_x = comp.data[y_min:y_max, x]
-        if zoomed_data_x.size > 0:
-            self.plot_across_x.set_limits(x_min=y_min,
-                                          x_max=y_max,
-                                          y_min=np.nanmin(zoomed_data_x) * 0.95,
-                                          y_max=np.nanmax(zoomed_data_x) * 1.05)
-        self.plot_across_x.update_style('line', line_visible=True,
-                                        markers_visible=False, color='gray', size=10)
-        self.plot_across_x.viewer.axis_x.label = 'Y (pix)'
-        self.plot_across_x.viewer.axis_y.label = y_label
-
-        self.plot_across_y.figure.title = f'Y={y}'
-        self.plot_across_y._update_data('line', x=range(comp.data.shape[1]), y=comp.data[y, :],
-                                        reset_lims=False)
-        zoomed_data_y = comp.data[y, x_min:x_max]
-        if zoomed_data_y.size > 0:
-            self.plot_across_y.set_limits(x_min=x_min,
-                                          x_max=x_max,
-                                          y_min=np.nanmin(zoomed_data_y) * 0.95,
-                                          y_max=np.nanmax(zoomed_data_y) * 1.05)
-        self.plot_across_y.update_style('line', line_visible=True,
-                                        markers_visible=False, color='gray', size=10)
-        self.plot_across_y.viewer.axis_x.label = 'X (pix)'
-        self.plot_across_y.viewer.axis_y.label = y_label
-
-        self.plot_available = True
+        vid = self.viewer.selected_id
+        self.angle = self.app._viewer_item_by_id(vid).get('canvas_angle', 0)
+        self.flip_horizontal = self.app._viewer_item_by_id(vid).get('canvas_flip_horizontal', False)
+
+    def _get_wcs_angles(self):
+        if not self.has_wcs:
+            raise ValueError("reference data does not have WCS, cannot determine orientation")
+        ref_data = self.ref_data
+        if ref_data is None:  # pragma: no cover
+            raise ValueError("no data loaded in viewer, cannot determine orientation")
+        _, _, _, _, _, _, degn, dege, flip = get_compass_info(ref_data.coords, ref_data.shape)
+        return degn, dege, flip
+
+    def reset(self):
+        """
+        Reset the rotation to an angle of 0 and no flip
+        """
+        self.angle = 0
+        self.flip_horizontal = False
+
+    def set_north_up_east_left(self):
+        """
+        Set the rotation angle and flip to achieve North up and East left according to the reference
+        image WCS.
+        """
+        degn, dege, flip = self._get_wcs_angles()
+        self.angle = -degn
+        self.flip_horizontal = flip
+
+    def set_north_up_east_right(self):
+        """
+        Set the rotation angle and flip to achieve North up and East right according to the
+        reference image WCS.
+        """
+        degn, dege, flip = self._get_wcs_angles()
+        self.angle = -degn
+        self.flip_horizontal = not flip
+
+    def vue_reset(self, *args, **kwargs):
+        self.reset()  # pragma: no cover
+
+    def vue_set_north_up_east_left(self, *args, **kwargs):
+        self.set_north_up_east_left()  # pragma: no cover
+
+    def vue_set_north_up_east_right(self, *args, **kwargs):
+        self.set_north_up_east_right()  # pragma: no cover
+
+    @observe('angle')
+    def _angle_changed(self, *args, **kwargs):
+        try:
+            angle = float(self.angle)
+        except ValueError:  # pragma: no cover
+            # empty string, etc
+            angle = 0
+
+        # Rotate selected viewer canvas. This changes zoom too.
+        self.app._viewer_item_by_id(self.viewer.selected_id)['canvas_angle'] = angle
+        # broadcast message (used by compass, etc)
+        self.hub.broadcast(CanvasRotationChangedMessage(self.viewer.selected_id,
+                                                        angle, self.flip_horizontal, sender=self))
+
+    @observe('flip_horizontal')
+    def _flip_changed(self, *args, **kwargs):
+        self.app._viewer_item_by_id(self.viewer.selected_id)['canvas_flip_horizontal'] = self.flip_horizontal  # noqa
+        self.hub.broadcast(CanvasRotationChangedMessage(self.viewer.selected_id,
+                                                        self.angle, self.flip_horizontal,
+                                                        sender=self))
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.vue` & `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.vue`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 <template>
   <j-tray-plugin
-    description='Press l to plot line profiles across X and Y under cursor. You can also manually enter X, Y and then click PLOT.'
+    :description="docs_description || 'Press l to plot line profiles across X and Y under cursor. You can also manually enter X, Y and then click PLOT.'"
     :link="docs_link || 'https://jdaviz.readthedocs.io/en/'+vdocs+'/'+config+'/plugins.html#line-profiles'"
     :uses_active_status="uses_active_status"
     @plugin-ping="plugin_ping($event)"
-    :popout_button="popout_button">
+    :popout_button="popout_button"
+    :scroll_to.sync="scroll_to">
 
     <plugin-viewer-select
       :items="viewer_items"
       :selected.sync="viewer_selected"
       label="Viewer"
       :show_if_single_entry="false"
       hint="Select a viewer to plot."
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/plugins/parsers.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/parsers.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from glue.core.data import Component, Data
 from gwcs.wcs import WCS as GWCS
 from stdatamodels import asdf_in_fits
 
 from jdaviz.core.registries import data_parser_registry
 from jdaviz.core.events import SnackbarMessage
-from jdaviz.utils import standardize_metadata, PRIHDR_KEY
+from jdaviz.utils import standardize_metadata, PRIHDR_KEY, _wcs_only_label
 
 try:
     from roman_datamodels import datamodels as rdd
 except ImportError:
     HAS_ROMAN_DATAMODELS = False
 else:
     HAS_ROMAN_DATAMODELS = True
@@ -26,15 +26,15 @@
 __all__ = ['parse_data']
 
 INFO_MSG = ("The file contains more viewable extensions. Add the '[*]' suffix"
             " to the file name to load all of them.")
 
 
 @data_parser_registry("imviz-data-parser")
-def parse_data(app, file_obj, ext=None, data_label=None):
+def parse_data(app, file_obj, ext=None, data_label=None, parent=None):
     """Parse a data file into Imviz.
 
     Parameters
     ----------
     app : `~jdaviz.app.Application`
         The application-level object used to reference the viewers.
 
@@ -70,35 +70,35 @@
             from skimage.color import rgb2gray, rgba2rgb
             im = imread(file_obj)
             if im.shape[2] == 4:
                 pf = rgb2gray(rgba2rgb(im))
             else:  # Assume RGB
                 pf = rgb2gray(im)
             pf = pf[::-1, :]  # Flip it
-            _parse_image(app, pf, data_label, ext=ext)
+            _parse_image(app, pf, data_label, ext=ext, parent=parent)
 
         elif file_obj_lower.endswith('.asdf'):
             try:
                 if HAS_ROMAN_DATAMODELS:
                     with rdd.open(file_obj) as pf:
-                        _parse_image(app, pf, data_label, ext=ext)
+                        _parse_image(app, pf, data_label, ext=ext, parent=parent)
             except TypeError:
                 # if roman_datamodels cannot parse the file, load it with asdf:
                 with asdf.open(file_obj) as af:
-                    _parse_image(app, af, data_label, ext=ext)
+                    _parse_image(app, af, data_label, ext=ext, parent=parent)
 
         elif file_obj_lower.endswith('.reg'):
             # This will load DS9 regions as Subset but only if there is already data.
             app._jdaviz_helper.load_regions_from_file(file_obj)
 
         else:  # Assume FITS
             with fits.open(file_obj) as pf:
-                _parse_image(app, pf, data_label, ext=ext)
+                _parse_image(app, pf, data_label, ext=ext, parent=parent)
     else:
-        _parse_image(app, file_obj, data_label, ext=ext)
+        _parse_image(app, file_obj, data_label, ext=ext, parent=parent)
 
 
 def get_image_data_iterator(app, file_obj, data_label, ext=None):
     """This function is for internal use, so other viz can also extract image data
     like Imviz does.
     """
 
@@ -142,15 +142,18 @@
 
     elif isinstance(file_obj, (fits.ImageHDU, fits.CompImageHDU, fits.PrimaryHDU)):
         # NOTE: ext is not used here. It only means something if HDUList is given.
         _validate_fits_image2d(file_obj)
         data_iter = _hdu_to_glue_data(file_obj, data_label)
 
     elif isinstance(file_obj, NDData):
-        data_iter = _nddata_to_glue_data(file_obj, data_label)
+        if file_obj.meta.get(_wcs_only_label, False):
+            data_iter = _wcsonly_to_glue_data(file_obj, data_label)
+        else:
+            data_iter = _nddata_to_glue_data(file_obj, data_label)
 
     elif isinstance(file_obj, np.ndarray):
         data_iter = _ndarray_to_glue_data(file_obj, data_label)
 
     # load Roman 2D datamodels:
     elif HAS_ROMAN_DATAMODELS and isinstance(file_obj, rdd.DataModel):
         data_iter = _roman_2d_to_glue_data(file_obj, data_label, ext=ext)
@@ -161,15 +164,15 @@
 
     else:
         raise NotImplementedError(f'Imviz does not support {file_obj}')
 
     return data_iter
 
 
-def _parse_image(app, file_obj, data_label, ext=None):
+def _parse_image(app, file_obj, data_label, ext=None, parent=None):
     if app is None:
         raise ValueError("app is None, cannot proceed")
     if data_label is None:
         data_label = app.return_data_label(file_obj, ext, alt_name="image_data")
     data_iter = get_image_data_iterator(app, file_obj, data_label, ext=ext)
 
     for data, data_label in data_iter:
@@ -177,18 +180,28 @@
             # keep a copy of the original bounding box so we can detect
             # when extrapolating beyond, but then remove the bounding box
             # so that image layers are not cropped.
             # NOTE: if extending this beyond GWCS, the mouseover logic
             # for outside_*_bounding_box should also be updated.
             data.coords._orig_bounding_box = data.coords.bounding_box
             data.coords.bounding_box = None
-        data_label = app.return_data_label(data_label, alt_name="image_data")
-        app.add_data(data, data_label)
+        if not data.meta.get(_wcs_only_label, False):
+            data_label = app.return_data_label(data_label, alt_name="image_data")
+
+        # TODO: generalize/centralize this for use in other configs too
+        if parent is not None and ext == 'DQ':
+            # nans are used to mark "good" flags in the DQ colormap, so
+            # convert DQ array to float to support nans:
+            cid = data.get_component("DQ")
+            data_arr = np.float32(cid.data)
+            data_arr[data_arr == 0] = np.nan
+            data.update_components({cid: data_arr})
+        app.add_data(data, data_label, parent=parent)
 
-    # Do not run link_image_data here. We do it at the end in Imviz.load_data()
+    # Do not link image data here. We do it at the end in Imviz.load_data()
 
 
 def _info_nextensions(app, file_obj):
     if _count_image2d_extensions(file_obj) > 1:
         info_msg = SnackbarMessage(INFO_MSG, color="info", timeout=8000, sender=app)
         app.hub.broadcast(info_msg)
 
@@ -408,15 +421,15 @@
 
 # ---- Functions that handle input from arrays -----
 
 def _nddata_to_glue_data(ndd, data_label):
     if ndd.data.ndim != 2:
         raise ValueError(f'Imviz cannot load this NDData with ndim={ndd.data.ndim}')
 
-    for attrib in ['data', 'mask', 'uncertainty']:
+    for attrib in ('data', 'mask', 'uncertainty'):
         arr = getattr(ndd, attrib)
         if arr is None:
             continue
         comp_label = attrib.upper()
         cur_label = f'{data_label}[{comp_label}]'
         cur_data = Data(label=cur_label)
         cur_data.meta.update(standardize_metadata(ndd.meta))
@@ -439,7 +452,20 @@
     if arr.ndim != 2:
         raise ValueError(f'Imviz cannot load this array with ndim={arr.ndim}')
 
     data = Data(label=data_label)
     component = Component.autotyped(arr)
     data.add_component(component=component, label='DATA')
     yield (data, data_label)
+
+
+# ---- Functions that handle WCS-only data -----
+
+def _wcsonly_to_glue_data(ndd, data_label):
+    """Return Data given NDData containing WCS-only data."""
+    arr = ndd.data
+    data = Data(label=data_label)
+    data.meta.update(standardize_metadata(ndd.meta))
+    data.coords = ndd.wcs
+    component = Component.autotyped(arr, units="")
+    data.add_component(component=component, label="DATA")
+    yield (data, data_label)
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.vue` & `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.vue`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 <template>
   <j-tray-plugin  
-    description="Rotate viewer canvas to any orientation (note: this does not affect the underlying data)."
+    :description="docs_description || 'Rotate viewer canvas to any orientation (note: this does not affect the underlying data).'"
     :link="docs_link || 'https://jdaviz.readthedocs.io/en/'+vdocs+'/'+config+'/plugins.html#canvas-rotation'"
     :disabled_msg="isChromium() ? '' : 'Image rotation is not supported by your browser. Please see our docs for more information.'"
-    :popout_button="popout_button">
+    :popout_button="popout_button"
+    :scroll_to.sync="scroll_to">
+
+    <v-alert type='warning'>
+      This plugin is deprecated in favor of rotation via the Orientation plugin and will be removed
+      in a future release.
+    </v-alert>
+
     <plugin-viewer-select
       :items="viewer_items"
       :selected.sync="viewer_selected"
       label="Viewer"
       hint="Select viewer."
     />
 
@@ -77,8 +84,8 @@
       }
       catch {
         return false
       }
     }
   }
 }
-</script>
+</script>
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/plugins/rotate_canvas/tests/test_rotate_canvas.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/rotate_canvas/tests/test_rotate_canvas.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/plugins/tools.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/tools.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,41 +4,28 @@
 
 from glue.config import viewer_tool
 from glue.viewers.common.tool import CheckableTool
 from glue_jupyter.bqplot.image import BqplotImageView
 from glue_jupyter.utils import debounced
 
 from jdaviz.core.tools import BoxZoom, PanZoom, _MatchedZoomMixin
+from jdaviz.configs.imviz.helper import get_top_layer_index
 
 __all__ = []
 
 ICON_DIR = os.path.join(os.path.dirname(__file__), '..', '..', '..', 'data', 'icons')
 
 
 class _ImvizMatchedZoomMixin(_MatchedZoomMixin):
     match_keys = ('x_min', 'x_max', 'y_min', 'y_max')
-    disable_matched_zoom_in_other_viewer = False
+    disable_matched_zoom_in_other_viewer = True
 
     def _is_matched_viewer(self, viewer):
         return isinstance(viewer, BqplotImageView)
 
-    def _post_activate(self):
-        # NOTE: For Imviz only.
-        # Set the reference data in other viewers to be the same as the current viewer.
-        # If adding the data to the viewer, make sure it is not actually shown since the
-        # user didn't request it.
-        for viewer in self._iter_matched_viewers(include_self=False):
-            if self.viewer.state.reference_data not in viewer.state.layers_data:
-                viewer.add_data(self.viewer.state.reference_data)
-                for layer in viewer.state.layers:
-                    if layer.layer is self.viewer.state.reference_data:
-                        layer.visible = False
-                        break
-            viewer.state.reference_data = self.viewer.state.reference_data
-
 
 @viewer_tool
 class ImagePanZoom(PanZoom):
     tool_id = 'jdaviz:imagepanzoom'
     tool_tip = 'Interactively pan (click-drag), zoom (scroll), and center (click)'
 
     def activate(self):
@@ -47,23 +34,26 @@
 
     def deactivate(self):
         self.viewer.remove_event_callback(self.on_click)
         super().deactivate()
 
     def on_click(self, data):
         # Find visible layers
-        visible_layers = [layer for layer in self.viewer.state.layers if layer.visible]
-        if len(visible_layers) == 0:
+        try:
+            i = get_top_layer_index(self.viewer)
+        except IndexError:
+            return
+        if i is None:
             return
 
         # Same data as mousemove event in Imviz viewer.
         # Any other config that wants this functionality has to have the following:
         #   viewer._get_real_xy()
         #   viewer.center_on() --> inherited from AstrowidgetsImageViewerMixin
-        image = visible_layers[0].layer
+        image = self.viewer.state.layers[i].layer
         x = data['domain']['x']
         y = data['domain']['y']
         if x is None or y is None:  # Out of bounds
             return
         x, y, _, _ = self.viewer._get_real_xy(image, x, y)
         self.viewer.center_on((x, y))
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/plugins/viewers.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/plugins/viewers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 
 import astropy.units as u
 from astropy.wcs.utils import pixel_to_pixel
 from astropy.visualization import ImageNormalize, LinearStretch, PercentileInterval
+from glue.core.link_helpers import LinkSame
 from glue_jupyter.bqplot.image import BqplotImageView
 
 from jdaviz.configs.imviz import wcs_utils
 from jdaviz.configs.imviz.helper import layer_is_image_data, get_top_layer_index
 from jdaviz.core.astrowidgets_api import AstrowidgetsImageViewerMixin
 from jdaviz.core.events import SnackbarMessage
 from jdaviz.core.helpers import data_has_valid_wcs
@@ -21,24 +22,26 @@
 class ImvizImageView(JdavizViewerMixin, BqplotImageView, AstrowidgetsImageViewerMixin):
     # categories: zoom resets, zoom, pan, subset, select tools, shortcuts
     tools_nested = [
                     ['jdaviz:homezoom', 'jdaviz:prevzoom'],
                     ['jdaviz:boxzoommatch', 'jdaviz:boxzoom'],
                     ['jdaviz:panzoommatch', 'jdaviz:imagepanzoom'],
                     ['bqplot:truecircle', 'bqplot:rectangle', 'bqplot:ellipse',
-                     'bqplot:circannulus', 'jdaviz:singlepixelregion'],
+                     'bqplot:circannulus'],
                     ['jdaviz:blinkonce', 'jdaviz:contrastbias'],
                     ['jdaviz:sidebar_plot', 'jdaviz:sidebar_export', 'jdaviz:sidebar_compass']
                 ]
 
     default_class = None
     _state_cls = FreezableBqplotImageViewerState
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
+        # provide reference from state back to viewer to use for zoom syncing
+        self.state._viewer = self
         self.init_astrowidgets_api()
         self._subscribe_to_layers_update()
 
         self.compass = None
         self.line_profile_xy = None
 
         self.add_event_callback(self.on_mouse_or_key_event, events=['keydown'])
@@ -79,17 +82,24 @@
             if key_pressed in ('b', 'B'):
                 self.blink_once(reversed=key_pressed=='B')  # noqa: E225
 
     def blink_once(self, reversed=False):
         # Simple blinking of images - this will make it so that only one
         # layer is visible at a time and cycles through the layers.
 
-        # Exclude Subsets: They are global
+        # Exclude Subsets (they are global) and children via associated data
+
+        def is_parent(data):
+            return self.session.jdaviz_app._get_assoc_data_parent(data.label) is None
+
         valid = [ilayer for ilayer, layer in enumerate(self.state.layers)
-                 if layer_is_image_data(layer.layer)]
+                 if layer_is_image_data(layer.layer) and is_parent(layer.layer)]
+        children = [ilayer for ilayer, layer in enumerate(self.state.layers)
+                    if layer_is_image_data(layer.layer) and not is_parent(layer.layer)]
+
         n_layers = len(valid)
 
         if n_layers == 1:
             msg = SnackbarMessage(
                 'Nothing to blink. Select a second image in the Data menu to use this feature.',
                 color='warning', sender=self)
             self.session.hub.broadcast(msg)
@@ -109,15 +119,20 @@
                 if not reversed:
                     delta = 1
                 else:
                     delta = -1
                 next_layer = valid[(valid.index(visible[-1]) + delta) % n_layers]
                 self.state.layers[next_layer].visible = True
 
-                for ilayer in (set(valid) - set([next_layer])):
+                # make invisible all parent layers other than the next layer:
+                layers_to_set_not_visible = set(valid) - set([next_layer])
+                # no child layers are visible by default:
+                layers_to_set_not_visible.update(set(children))
+
+                for ilayer in layers_to_set_not_visible:
                     self.state.layers[ilayer].visible = False
 
                 # We can display the active data label in Compass plugin.
                 self.set_compass(self.state.layers[next_layer].layer)
 
                 # Update line profile plots too.
                 if self.line_profile_xy is None:
@@ -132,27 +147,43 @@
     def on_limits_change(self, *args):
         try:
             i = get_top_layer_index(self)
         except IndexError:
             if self.compass is not None:
                 self.compass.clear_compass()
             return
+        if i is None:
+            return
         self.set_compass(self.state.layers[i].layer)
 
     @property
     def top_visible_data_label(self):
         """Data label of the top visible layer in the viewer."""
         try:
             i = get_top_layer_index(self)
         except IndexError:
             data_label = ''
         else:
-            data_label = self.state.layers[i].layer.label
+            if i is None:
+                data_label = ''
+            else:
+                data_label = self.state.layers[i].layer.label
         return data_label
 
+    @property
+    def first_loaded_data(self):
+        """Data that is first loaded into the viewer.
+        This may not be the visible layer.
+        Returns `None` if no real data is loaded.
+        """
+        for lyr in self.layers:
+            data = lyr.layer
+            if layer_is_image_data(data):
+                return data
+
     def _get_real_xy(self, image, x, y, reverse=False):
         """Return real (X, Y) position and status in case of dithering as well as whether the
         results were within the bounding box of the reference data or required possibly inaccurate
         extrapolation.
 
         ``coords_status`` is for ``CoordsInfo`` coords handling only.
         When `True`, it sets the coords, otherwise it resets.
@@ -165,15 +196,15 @@
         unreliable_world = False
         unreliable_pixel = False
         if data_has_valid_wcs(image):
             # Convert these to a SkyCoord via WCS - note that for other datasets
             # we aren't actually guaranteed to get a SkyCoord out, just for images
             # with valid celestial WCS
             try:
-                link_type = self.get_link_type(image.label)
+                link_type = self.get_link_type(image.label).lower()
 
                 # Convert X,Y from reference data to the one we are actually seeing.
                 # world_to_pixel return scalar ndarray that we need to convert to float.
                 if link_type == 'wcs':
                     if not reverse:
                         outside_ref_bounding_box = wcs_utils.data_outside_gwcs_bounding_box(
                             self.state.reference_data, x, y)
@@ -205,19 +236,21 @@
     def _get_zoom_limits(self, image):
         """Return a list of ``(x, y)`` that defines four corners of
         the zoom box for a given image.
         This is needed because viewer values are only based on reference
         image, which can be inaccurate if given image is dithered and
         they are linked by WCS.
         """
-        if data_has_valid_wcs(image) and self.get_link_type(image.label) == 'wcs':
-            # Convert X,Y from reference data to the one we are actually seeing.
-            x = image.coords.world_to_pixel(self.state.reference_data.coords.pixel_to_world(
+        if self.state.reference_data.meta.get('_WCS_ONLY', False):
+            corner_world_coords = self.state.reference_data.coords.pixel_to_world(
                 (self.state.x_min, self.state.x_min, self.state.x_max, self.state.x_max),
-                (self.state.y_min, self.state.y_max, self.state.y_max, self.state.y_min)))
+                (self.state.y_min, self.state.y_max, self.state.y_max, self.state.y_min)
+            )
+            # Convert X,Y from reference data to the one we are actually seeing.
+            x = image.coords.world_to_pixel(corner_world_coords)
             zoom_limits = np.array(list(zip(x[0], x[1])))
         else:
             zoom_limits = np.array(((self.state.x_min, self.state.y_min),
                                     (self.state.x_min, self.state.y_max),
                                     (self.state.x_max, self.state.y_max),
                                     (self.state.x_max, self.state.y_min)))
 
@@ -264,44 +297,77 @@
         ----------
         data_label : str
             Data label to look up.
 
         Returns
         -------
         link_type : {'pixels', 'wcs', 'self'}
-            One of the link types accepted by :func:`~jdaviz.configs.imviz.helper.link_image_data`
+            One of the link types accepted by the Orientation plugin
             or ``'self'`` if the data label belongs to the reference data itself.
 
         Raises
         ------
         ValueError
             Link look-up failed.
 
         """
         if len(self.session.application.data_collection) == 0:
             raise ValueError('No reference data for link look-up')
 
-        # TODO: Brett Morris might want to look at this for
-        # https://github.com/spacetelescope/jdaviz/pull/2179
-        #     ref_label = self.state.reference_data ???
-        #
-        # The original links were created against data_collection[0], not necessarily
-        # against the current viewer reference_data
-        ref_label = self.session.application.data_collection[0].label
+        ref_label = getattr(self.state.reference_data, 'label', None)
+        if data_label == ref_label:
+            return 'self'
+
+        if ref_label in self.state.wcs_only_layers:
+            return 'wcs'
+
+        link_type = None
+        for elink in self.session.application.data_collection.external_links:
+            elink_labels = (elink.data1.label, elink.data2.label)
+            if data_label in elink_labels and ref_label in elink_labels:
+                if isinstance(elink, LinkSame):  # Assumes WCS link never uses LinkSame
+                    link_type = 'pixels'
+                else:  # If not pixels, must be WCS
+                    link_type = 'wcs'
+                break  # Might have duplicate, just grab first match
+
+        if link_type is None:
+            raise ValueError(f'{data_label} not found in data collection external links')
+
+        return link_type
+
+    def _get_fov(self, wcs=None):
+        if wcs is None:
+            wcs = self.state.reference_data.coords
+        if self.jdaviz_app._link_type != "wcs" or wcs is None:
+            return
 
-        return self.jdaviz_helper.get_link_type(ref_label, data_label)
+        # compute the mean of the height and width of the
+        # viewer's FOV on ``data`` in world units:
+        x_corners = [
+            self.state.x_min,
+            self.state.x_max,
+            self.state.x_min
+        ]
+        y_corners = [
+            self.state.y_min,
+            self.state.y_min,
+            self.state.y_max
+        ]
+
+        sky_corners = wcs.pixel_to_world(x_corners, y_corners)
+        height_sky = abs(sky_corners[0].separation(sky_corners[2]))
+        width_sky = abs(sky_corners[0].separation(sky_corners[1]))
+        fov_sky = u.Quantity([height_sky, width_sky]).mean()
+        return fov_sky
 
     def _get_center_skycoord(self, data=None):
-        if data is None:
-            data = self.state.reference_data
         # get SkyCoord for the center of ``data`` in this viewer:
-        width = self.state.x_max - self.state.x_min
-        height = self.state.y_max - self.state.y_min
-        x_cen = self.state.x_min + (width * 0.5)
-        y_cen = self.state.y_min + (height * 0.5)
-        x_cen, y_cen = self._get_real_xy(
-            data, x_cen, y_cen
-        )[:2]
-        sky_cen = data.coords.pixel_to_world(
-            x_cen * u.pix, y_cen * u.pix
-        )
-        return sky_cen
+        x_cen = (self.state.x_min + self.state.x_max) * 0.5
+        y_cen = (self.state.y_min + self.state.y_max) * 0.5
+
+        if (self.jdaviz_app._link_type == "wcs" or data is None
+                or data.label == self.state.reference_data.label):
+            return self.state.reference_data.coords.pixel_to_world(x_cen, y_cen)
+
+        if data.coords is not None:
+            return data.coords.pixel_to_world(x_cen, y_cen)
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/tests/data/gauss100_fits_wcs.fits` & `jdaviz-3.9.0/jdaviz/configs/imviz/tests/data/gauss100_fits_wcs.fits`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/tests/data/gauss100_fits_wcs_block_reduced.fits` & `jdaviz-3.9.0/jdaviz/configs/imviz/tests/data/gauss100_fits_wcs_block_reduced.fits`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/tests/data/gauss100_fits_wcs_block_reduced_rotated.fits` & `jdaviz-3.9.0/jdaviz/configs/imviz/tests/data/gauss100_fits_wcs_block_reduced_rotated.fits`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/tests/data/miri_i2d_lonlat_gwcs.asdf` & `jdaviz-3.9.0/jdaviz/configs/imviz/tests/data/miri_i2d_lonlat_gwcs.asdf`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_astrowidgets_api.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_astrowidgets_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,36 +92,38 @@
         with pytest.raises(AttributeError, match='does not have a valid WCS'):
             self.viewer.offset_by(dsky, dsky)
 
 
 class TestCenter(BaseImviz_WCS_WCS):
 
     def test_center_on_pix(self):
-        self.imviz.link_data(link_type='wcs', error_on_fail=True)
+        self.imviz.link_data(link_type='wcs')
 
         # This is the second loaded data that is dithered by 1-pix.
         self.viewer.center_on((0, 0))
+        expected_position = [-6.75, 4.25, -5.75, 5.25]
+        rtol = 1e-4
         assert_allclose((self.viewer.state.x_min, self.viewer.state.x_max,
                          self.viewer.state.y_min, self.viewer.state.y_max),
-                        (-6, 4, -5, 5))
+                        expected_position, rtol=rtol)
 
         # This is the first data.
         self.viewer.blink_once()
         self.viewer.center_on((0, 0))
         assert_allclose((self.viewer.state.x_min, self.viewer.state.x_max,
                          self.viewer.state.y_min, self.viewer.state.y_max),
-                        (-5, 5, -5, 5))
+                        [-5.75, 5.25, -5.75, 5.25], rtol=rtol)
 
         # Centering by sky on second data.
         self.viewer.blink_once()
         sky = self.wcs_2.pixel_to_world(0, 0)
         self.viewer.center_on(sky)
         assert_allclose((self.viewer.state.x_min, self.viewer.state.x_max,
                          self.viewer.state.y_min, self.viewer.state.y_max),
-                        (-6, 4, -5, 5))
+                        expected_position, rtol=rtol)
 
 
 class TestZoom(BaseImviz_WCS_NoWCS):
 
     @pytest.mark.parametrize('val', (0, -0.1, 'foo', [1, 2]))
     def test_invalid_zoom_level(self, val):
         with pytest.raises(ValueError, match='Unsupported zoom level'):
@@ -176,15 +178,15 @@
 class TestCmapStretchCuts(BaseImviz_WCS_NoWCS):
 
     def test_colormap_options(self):
         assert self.viewer.colormap_options == [
             'Gray', 'Viridis', 'Plasma', 'Inferno', 'Magma', 'Purple-Blue',
             'Yellow-Green-Blue', 'Yellow-Orange-Red', 'Red-Purple', 'Blue-Green',
             'Hot', 'Red-Blue', 'Red-Yellow-Blue', 'Purple-Orange', 'Purple-Green',
-            'Rainbow', 'Seismic',
+            'Random', 'Rainbow', 'Seismic',
             'Reversed: Gray', 'Reversed: Viridis', 'Reversed: Plasma', 'Reversed: Inferno',
             'Reversed: Magma', 'Reversed: Hot', 'Reversed: Rainbow']
 
     def test_invalid_colormap(self):
         with pytest.raises(ValueError, match='Invalid colormap'):
             self.viewer.set_colormap('foo')
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_catalogs.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_catalogs.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,33 +31,29 @@
 
 
 @pytest.mark.remote_data
 class TestCatalogs:
 
     # testing that the plugin search does not crash when no data/image is provided
     def test_plugin_no_image(self, imviz_helper):
-        self.imviz = imviz_helper
-
-        catalogs_plugin = self.imviz.app.get_tray_item_from_name('imviz-catalogs')
+        catalogs_plugin = imviz_helper.plugins["Catalog Search"]._obj
         catalogs_plugin.plugin_opened = True
         # running the search without any data loaded into Imviz
         catalogs_plugin.vue_do_search()
 
         assert not catalogs_plugin.results_available
 
     # testing that variables update correctly when the image/data provided does not have results
     def test_plugin_image_no_result(self, imviz_helper, image_2d_wcs):
         arr = np.ones((10, 10))
         ndd = NDData(arr, wcs=image_2d_wcs)
 
         imviz_helper.load_data(ndd, data_label='no_results_data')
 
-        self.imviz = imviz_helper
-
-        catalogs_plugin = self.imviz.app.get_tray_item_from_name('imviz-catalogs')
+        catalogs_plugin = imviz_helper.plugins["Catalog Search"]._obj
         catalogs_plugin.plugin_opened = True
         catalogs_plugin.vue_do_search()
 
         # number of results should be 0
         assert catalogs_plugin.results_available
         assert catalogs_plugin.number_of_results == 0
 
@@ -84,54 +80,50 @@
                             'CD2_1': 7.74973322238e-05,
                             'CD2_2': 7.80788034973e-05,
                             'CRPIX2': 745.0,
                             'CRVAL2': 1.54470013629,
                             'NAXIS2': 1489})
         imviz_helper.load_data(hdu1, data_label='has_wcs')
 
-        self.imviz = imviz_helper
-
-        catalogs_plugin = self.imviz.app.get_tray_item_from_name('imviz-catalogs')
+        catalogs_plugin = imviz_helper.plugins["Catalog Search"]._obj
         catalogs_plugin.plugin_opened = True
         # This basically calls the following under the hood:
         #   skycoord_center = SkyCoord(6.62754354, 1.54466139, unit="deg")
         #   zoom_radius = r_max = 3 * u.arcmin
         #   query_region_result = SDSS.query_region(skycoord_center, radius=zoom_radius, ...)
-        catalogs_plugin.vue_do_search()
+        catalogs_plugin.search(error_on_fail=True)
 
         # number of results should be > 500 or so
         # Answer was determined by running the search with the image in the notebook.
         assert catalogs_plugin.results_available
         assert catalogs_plugin.number_of_results > 500
         prev_results = catalogs_plugin.number_of_results
 
         # testing that every variable updates accordingly when markers are cleared
         catalogs_plugin.vue_do_clear()
 
         assert not catalogs_plugin.results_available
 
         # test loading from file
         table = imviz_helper.app._catalog_source_table
-        skycoord_table = SkyCoord(table['ra'],
-                                  table['dec'],
-                                  unit='deg')
+        skycoord_table = SkyCoord(table['ra'], table['dec'], unit='deg')
         qtable = QTable({'sky_centroid': skycoord_table})
         tmp_file = tmp_path / 'test.ecsv'
         qtable.write(tmp_file, overwrite=True)
 
         catalogs_plugin.from_file = str(tmp_file)
         # setting filename from API will automatically set catalog to 'From File...'
         assert catalogs_plugin.catalog.selected == 'From File...'
         catalogs_plugin.vue_do_search()
         assert catalogs_plugin.results_available
         assert catalogs_plugin.number_of_results == prev_results
 
 
 def test_from_file_parsing(imviz_helper, tmp_path):
-    catalogs_plugin = imviz_helper.app.get_tray_item_from_name('imviz-catalogs')
+    catalogs_plugin = imviz_helper.plugins["Catalog Search"]._obj
 
     # _on_file_path_changed is fired when changing the selection in the file dialog
     catalogs_plugin.catalog._on_file_path_changed({'new': './invalid_path'})
     assert catalogs_plugin.from_file_message == 'File path does not exist'
 
     # observe('from_file') is fired when setting from_file from the API or via import_file
     # (or after clicking select in the file dialog)
@@ -163,22 +155,22 @@
     tbl.write(tbl_file, overwrite=True)
     n_entries = len(tbl)
 
     ndd = NDData(np.ones((10, 10)), wcs=image_2d_wcs)
     imviz_helper.load_data(ndd, data_label='data_with_wcs')
     assert len(imviz_helper.app.data_collection) == 1
 
-    catalogs_plugin = imviz_helper.plugins['Catalog Search']
-    catalogs_plugin._obj.from_file = tbl_file
-    catalogs_plugin._obj.catalog_selected = 'From File...'
-    out_tbl = catalogs_plugin._obj.search()
+    catalogs_plugin = imviz_helper.plugins['Catalog Search']._obj
+    catalogs_plugin.from_file = tbl_file
+    catalogs_plugin.catalog_selected = 'From File...'
+    out_tbl = catalogs_plugin.search(error_on_fail=True)
     assert len(out_tbl) == n_entries
-    assert catalogs_plugin._obj.number_of_results == n_entries
+    assert catalogs_plugin.number_of_results == n_entries
     assert len(imviz_helper.app.data_collection) == 2  # image + markers
 
-    catalogs_plugin._obj.clear()
-    assert not catalogs_plugin._obj.results_available
+    catalogs_plugin.clear()
+    assert not catalogs_plugin.results_available
     assert len(imviz_helper.app.data_collection) == 2  # markers still there, just hidden
 
-    catalogs_plugin._obj.clear(hide_only=False)
-    assert not catalogs_plugin._obj.results_available
+    catalogs_plugin.clear(hide_only=False)
+    assert not catalogs_plugin.results_available
     assert len(imviz_helper.app.data_collection) == 1  # markers gone for good
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_footprints.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_footprints.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_helper.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_line_profile_xy.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_line_profile_xy.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_linking.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_linking.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 from astropy.table import Table
 from astropy.wcs import WCS
 from glue.core.link_helpers import LinkSame
-from glue.plugins.wcs_autolinking.wcs_autolinking import OffsetLink, WCSLink
+from glue.plugins.wcs_autolinking.wcs_autolinking import AffineLink, OffsetLink, WCSLink
 from numpy.testing import assert_allclose
 from regions import PixCoord, CirclePixelRegion, PolygonPixelRegion
 
 from jdaviz.configs.imviz.helper import get_reference_image_data
 from jdaviz.configs.imviz.tests.utils import (
     BaseImviz_WCS_NoWCS, BaseImviz_WCS_WCS, BaseImviz_WCS_GWCS, BaseImviz_GWCS_GWCS)
 
@@ -14,56 +14,49 @@
 class BaseLinkHandler:
 
     def check_all_pixel_links(self):
         links = self.imviz.app.data_collection.external_links
         assert len(links) == 2
         assert all([isinstance(link, LinkSame) for link in links])
 
+    def check_all_wcs_links(self):
+        links = self.imviz.app.data_collection.external_links
+        assert len(links) == 3
+        assert all([isinstance(link, (AffineLink, OffsetLink)) for link in links])
+
     def test_pixel_linking(self):
-        self.imviz.link_data(link_type='pixels', error_on_fail=True)
+        self.imviz.link_data(link_type='pixels')
         self.check_all_pixel_links()
 
     @property
     def default_viewer_limits(self):
         return (self.imviz.default_viewer._obj.state.x_min,
                 self.imviz.default_viewer._obj.state.x_max,
                 self.imviz.default_viewer._obj.state.y_min,
                 self.imviz.default_viewer._obj.state.y_max)
 
 
 class TestLink_WCS_NoWCS(BaseImviz_WCS_NoWCS, BaseLinkHandler):
 
     def test_wcslink_fallback_pixels(self):
-        self.imviz.link_data(link_type='wcs', error_on_fail=True)
-        self.check_all_pixel_links()
+        self.imviz.link_data(link_type='wcs')
 
-        assert self.viewer.get_link_type('has_wcs[SCI,1]') == 'self'
-        assert self.viewer.get_link_type('no_wcs[SCI,1]') == 'pixels'
+        assert self.viewer.get_link_type('has_wcs[SCI,1]') == 'wcs'
 
         # Also check the coordinates display: Last loaded is on top.
 
         label_mouseover = self.imviz.app.session.application._tools['g-coords-info']
         label_mouseover._viewer_mouse_event(self.viewer,
                                             {'event': 'mousemove', 'domain': {'x': 0, 'y': 0}})
-        assert label_mouseover.as_text() == ('Pixel x=00.0 y=00.0 Value +0.00000e+00', '', '')
 
-        # blink image through keypress
-        self.viewer.on_mouse_or_key_event({'event': 'keydown', 'key': 'b',
-                                           'domain': {'x': 0, 'y': 0}})
-        assert label_mouseover.as_text() == ('Pixel x=00.0 y=00.0 Value +0.00000e+00',
-                                             'World 22h30m04.8674s -20d49m59.9990s (ICRS)',
-                                             '337.5202808000 -20.8333330600 (deg)')
-
-    def test_wcslink_nofallback_noerror(self):
-        self.imviz.link_data(link_type='wcs', wcs_fallback_scheme=None)
-        self.check_all_pixel_links()  # Keeps old links because operation failed silently
-
-    def test_wcslink_nofallback_error(self):
-        with pytest.raises(AttributeError, match='pixel_n_dim'):
-            self.imviz.link_data(link_type='wcs', wcs_fallback_scheme=None, error_on_fail=True)
+        assert label_mouseover.as_text() == (
+            'Pixel x=00.3 y=00.2 Value +0.00000e+00',
+            'World 22h30m04.8496s -20d49m59.7490s (ICRS)',
+            '337.5202064976 -20.8332636155 (deg)'
+        )
 
 
 class TestLink_WCS_FakeWCS(BaseImviz_WCS_NoWCS, BaseLinkHandler):
 
     def test_badwcs_no_crash(self):
         # There is WCS but it is non-celestial
         self.imviz.app.data_collection[1].coords = WCS(naxis=2)
@@ -91,46 +84,37 @@
 
 class TestLink_WCS_WCS(BaseImviz_WCS_WCS, BaseLinkHandler):
 
     def test_wcslink_affine_with_extras(self):
         orig_pixel_limits = self.default_viewer_limits
         assert_allclose(orig_pixel_limits, (-0.5, 9.5, -0.5, 9.5))
 
-        self.imviz.link_data(link_type='wcs', wcs_fallback_scheme=None, error_on_fail=True)
+        self.imviz.link_data(link_type='wcs', wcs_fallback_scheme=None)
         links = self.imviz.app.data_collection.external_links
-        assert len(links) == 1
-        assert isinstance(links[0], OffsetLink)
-
+        assert len(links) == 2
+        assert isinstance(links[0], (AffineLink, OffsetLink))
         assert self.viewer.get_link_type('has_wcs_2[SCI,1]') == 'wcs'
 
-        # linking should not change axes limits, but should when resetting
-        assert_allclose(self.default_viewer_limits, orig_pixel_limits)
-        self.imviz.default_viewer.reset_limits()
-        assert_allclose(self.default_viewer_limits, (-1.5, 9.5, -1, 10))
-
         # Customize display on second image (last loaded).
         self.viewer.set_colormap('Viridis')
         self.viewer.stretch = 'sqrt'
         self.viewer.cuts = (0, 100)
 
         # Add subsets, both interactive and static.
         self.imviz._apply_interactive_region('bqplot:truecircle', (1.5, 2.5), (3.6, 4.6))
-        self.imviz.load_regions([CirclePixelRegion(center=PixCoord(x=6, y=2), radius=5),
-                                 PolygonPixelRegion(vertices=PixCoord(x=[1, 2, 2], y=[1, 1, 2])),
-                                 PolygonPixelRegion(vertices=PixCoord(x=[2, 3, 3], y=[2, 2, 3]))])
+        self.imviz.load_regions([
+            CirclePixelRegion(center=PixCoord(x=6, y=2), radius=5).to_sky(self.wcs_1),
+            PolygonPixelRegion(vertices=PixCoord(x=[1, 2, 2], y=[1, 1, 2])).to_sky(self.wcs_1),
+            PolygonPixelRegion(vertices=PixCoord(x=[2, 3, 3], y=[2, 2, 3])).to_sky(self.wcs_1)])
 
         # Add markers.
         tbl = Table({'x': (0, 0), 'y': (0, 1)})
         self.viewer.add_markers(tbl, marker_name='xy_markers')
         assert 'xy_markers' in self.imviz.app.data_collection.labels
 
-        # Run linking again with the same options as before (otherwise would fail with an error
-        # since markers now exist)
-        self.imviz.link_data(link_type='wcs', wcs_fallback_scheme=None, error_on_fail=True)
-
         # Ensure display is still customized.
         assert self.viewer.state.layers[1].cmap.name == 'viridis'
         assert self.viewer.state.layers[1].stretch == 'sqrt'
         assert_allclose((self.viewer.state.layers[1].v_min, self.viewer.state.layers[1].v_max),
                         (0, 100))
 
         # Ensure subsets are still there.
@@ -146,197 +130,137 @@
 
         # Pan/zoom.
         self.viewer.center_on((5, 5))
         self.viewer.zoom_level = 0.789
         ans = (self.viewer.state.x_min, self.viewer.state.y_min,
                self.viewer.state.x_max, self.viewer.state.y_max)
 
-        # Run linking again, does not matter what kind.
-        self.imviz.link_data(link_type='wcs', wcs_fallback_scheme=None, error_on_fail=True)
-
         # Ensure pan/zoom does not change when markers are not present.
         assert_allclose((self.viewer.state.x_min, self.viewer.state.y_min,
                         self.viewer.state.x_max, self.viewer.state.y_max), ans)
 
         # Also check the coordinates display: Last loaded is on top.
 
         label_mouseover = self.imviz.app.session.application._tools['g-coords-info']
         label_mouseover._viewer_mouse_event(self.viewer,
                                             {'event': 'mousemove',
                                              'domain': {'x': 0, 'y': 0}})
 
         lmtext = label_mouseover.as_text()
-        assert lmtext[0] in ('Pixel x=01.0 y=00.0 Value +1.00000e+00',
-                             'Pixel x=01.0 y=-0.0 Value +1.00000e+00')
-        assert lmtext[1:] == ('World 22h30m04.8674s -20d49m59.9990s (ICRS)',
-                              '337.5202808000 -20.8333330600 (deg)')
+        assert lmtext[0] == 'Pixel x=01.3 y=00.2 Value +1.00000e+00'
+        assert lmtext[1:] == ('World 22h30m04.8496s -20d49m59.7490s (ICRS)',
+                              '337.5202064976 -20.8332636155 (deg)')
 
         # blink image through clicking with blink tool
         self.viewer.toolbar.active_tool_id = 'jdaviz:blinkonce'
         self.viewer.toolbar.active_tool.on_click({'event': 'click', 'domain': {'x': 0, 'y': 0}})
-        assert label_mouseover.as_text() == ('Pixel x=00.0 y=00.0 Value +1.00000e+00',
-                                             'World 22h30m04.8674s -20d49m59.9990s (ICRS)',
-                                             '337.5202808000 -20.8333330600 (deg)')
+        assert label_mouseover.as_text()[0] == 'Pixel x=00.3 y=00.2 Value +1.00000e+00'
+        assert label_mouseover.as_text()[1:] == ('World 22h30m04.8496s -20d49m59.7490s (ICRS)',
+                                                 '337.5202064976 -20.8332636155 (deg)')
 
         # Changing link type will raise an error
-        with pytest.raises(ValueError, match="cannot change link_type"):
-            self.imviz.link_data(link_type='pixels', wcs_fallback_scheme=None, error_on_fail=True)
+        with pytest.raises(ValueError, match=".*only be changed after existing subsets are deleted"):  # noqa: E501
+            self.imviz.link_data(link_type='pixels', wcs_fallback_scheme=None)
 
         self.viewer.reset_markers()
-        self.imviz.link_data(link_type='pixels', wcs_fallback_scheme=None, error_on_fail=True)
+        self.imviz.plugins["Orientation"].delete_subsets()
+        self.imviz.link_data(link_type='pixels', wcs_fallback_scheme=None)
         assert 'xy_markers' not in self.imviz.app.data_collection.labels
         assert len(self.viewer._marktags) == 0
 
     def test_wcslink_fullblown(self):
-        self.imviz.link_data(link_type='wcs', wcs_fallback_scheme=None, wcs_use_affine=False,
-                             error_on_fail=True)
+        self.imviz.link_data(link_type='wcs', wcs_fallback_scheme=None, wcs_use_affine=False)
         links = self.imviz.app.data_collection.external_links
-        assert len(links) == 1
+        assert len(links) == 2
         assert isinstance(links[0], WCSLink)
-        assert self.viewer.get_link_type('has_wcs_1[SCI,1]') == 'self'
+        assert self.viewer.get_link_type('has_wcs_1[SCI,1]') == 'wcs'
         assert self.viewer.get_link_type('has_wcs_2[SCI,1]') == 'wcs'
 
     # Also test other exception handling here.
 
     def test_invalid_inputs(self):
-        with pytest.raises(ValueError, match='link_type'):
+        with pytest.raises(KeyError):
             self.imviz.link_data(link_type='foo')
 
-        with pytest.raises(ValueError, match='wcs_fallback_scheme'):
-            self.imviz.link_data(link_type='wcs', wcs_fallback_scheme='foo')
-
         with pytest.raises(ValueError, match='not found in data collection external links'):
             self.viewer.get_link_type('foo')
 
 
 class TestLink_WCS_GWCS(BaseImviz_WCS_GWCS):
 
     def test_wcslink_rotated(self):
         # FITS WCS will be reference, GWCS is rotated, no_wcs linked by pixel to ref.
-        self.imviz.link_data(link_type='wcs', error_on_fail=True)
+        self.imviz.link_data(link_type='wcs')
 
         # The zoom box for GWCS is now a rotated rombus.
         fits_wcs_zoom_limits = self.viewer._get_zoom_limits(
             self.imviz.app.data_collection['fits_wcs[DATA]'])
         gwcs_zoom_limits = self.viewer._get_zoom_limits(
             self.imviz.app.data_collection['gwcs[DATA]'])
-        no_wcs_zoom_limits = self.viewer._get_zoom_limits(
-            self.imviz.app.data_collection['no_wcs'])
         assert_allclose(fits_wcs_zoom_limits,
-                        ((-0.972136, 0.027864), (-0.972136, 8.972136),
-                         (7.972136, 8.972136), (7.972136, 0.027864)), rtol=1e-5)
+                        [[-1.590838, -0.423662],
+                         [-1.826862, 9.896219],
+                         [8.590838, 9.423662],
+                         [8.826862, -0.896219]], rtol=1e-5)
         assert_allclose(gwcs_zoom_limits,
-                        ((3.245117, 10.549265), (10.688389, 4.95208),
-                         (6.100057, -2.357782), (-1.343215, 3.239403)), rtol=1e-5)
-        assert_allclose(no_wcs_zoom_limits, fits_wcs_zoom_limits)
+                        [[3.186753, 11.337468],
+                         [11.895862, 5.072343],
+                         [6.158421, -3.145985],
+                         [-2.550688, 3.119141]], rtol=1e-5)
 
         # Also check the coordinates display: Last loaded is on top.
-        # Cycle order: no_wcs, FITS WCS, GWCS
-
+        # Cycle order: GWCS, FITS WCS
         label_mouseover = self.imviz.app.session.application._tools['g-coords-info']
-        label_mouseover._viewer_mouse_event(self.viewer,
-                                            {'event': 'mousemove', 'domain': {'x': 0, 'y': 0}})
-        assert label_mouseover.as_text() == ('Pixel x=00.0 y=00.0 Value +1.00000e+00', '', '')
-        assert not label_mouseover.row1_unreliable
-        assert not label_mouseover.row2_unreliable
-        assert not label_mouseover.row3_unreliable
-
-        self.viewer.on_mouse_or_key_event({'event': 'keydown', 'key': 'b',
-                                           'domain': {'x': 0, 'y': 0}})
-        assert label_mouseover.as_text() == ('Pixel x=00.0 y=00.0 Value +1.00000e+00 electron / s',
-                                             'World 00h14m19.6141s -30d23m31.4091s (ICRS)',
-                                             '3.5817255823 -30.3920580740 (deg)')
-        assert not label_mouseover.row1_unreliable
-        assert not label_mouseover.row2_unreliable
-        assert not label_mouseover.row3_unreliable
-
-        # viewer, not label_mouseover event
-        self.viewer.on_mouse_or_key_event({'event': 'keydown', 'key': 'b',
-                                           'domain': {'x': 0, 'y': 0}})
+        xy = self.viewer._get_real_xy(self.imviz.app.data_collection[0], 0, 0, reverse=True)
+        label_mouseover._viewer_mouse_event(
+            self.viewer, {'event': 'mousemove', 'domain': {'x': xy[0], 'y': xy[1]}})
         assert label_mouseover.as_text() == ('Pixel x=02.7 y=09.8',
                                              'World 00h14m19.6141s -30d23m31.4091s (ICRS)',
                                              '3.5817255823 -30.3920580740 (deg)')
         assert not label_mouseover.row1_unreliable
         assert not label_mouseover.row2_unreliable
         assert not label_mouseover.row3_unreliable
 
-        # Make sure GWCS now can extrapolate. Domain x,y is for FITS WCS data
-        # but they are linked by WCS.
-        label_mouseover._viewer_mouse_event(self.viewer,
-                                            {'event': 'mousemove',
-                                             'domain': {'x': 11.281551269520731,
-                                                        'y': 2.480347927198246}})
+        # Make sure GWCS now can extrapolate.
+        xy = self.viewer._get_real_xy(self.imviz.app.data_collection[1], -1, -1, reverse=True)
+        label_mouseover._viewer_mouse_event(
+            self.viewer, {'event': 'mousemove', 'domain': {'x': xy[0], 'y': xy[1]}})
         assert label_mouseover.as_text() == ('Pixel x=-1.0 y=-1.0',
                                              'World 00h14m19.5829s -30d23m30.9860s (ICRS)',
                                              '3.5815955408 -30.3919405616 (deg)')
         # FITS WCS is reference data and has no concept of bounding box
         # but cursor is outside GWCS bounding box
         assert label_mouseover.row1_unreliable
         assert label_mouseover.row2_unreliable
         assert label_mouseover.row3_unreliable
 
-
-class TestLink_GWCS_GWCS(BaseImviz_GWCS_GWCS):
-    def test_wcslink_offset(self):
-        self.imviz.link_data(link_type='wcs', error_on_fail=True)
-
-        # Check the coordinates display: Last loaded is on top.
-        # Within bounds of non-reference image but out of bounds of reference image.
-        label_mouseover = self.imviz.app.session.application._tools['g-coords-info']
-        label_mouseover._viewer_mouse_event(self.viewer,
-                                            {'event': 'mousemove', 'domain': {'x': 10, 'y': 3}})
-        lmtext = label_mouseover.as_text()
-        assert lmtext[0] in ('Pixel x=07.0 y=00.0 Value +0.00000e+00',
-                             'Pixel x=07.0 y=-0.0 Value +0.00000e+00')
-        assert lmtext[1:] == ('World 00h14m19.6291s -30d23m30.9692s (ICRS)',
-                              '3.5817877198 -30.3919358920 (deg)')
-
-        assert label_mouseover.row1_unreliable
-        assert label_mouseover.row2_unreliable
-        assert label_mouseover.row3_unreliable
-
-        # Non-reference image out of bounds of its own bounds but not of the
-        # reference image's bounds. Head hurting yet?
-        label_mouseover._viewer_mouse_event(self.viewer,
-                                            {'event': 'mousemove', 'domain': {'x': 0.5, 'y': 0.5}})
-        assert label_mouseover.as_text() == ('Pixel x=-2.5 y=-2.5',
-                                             'World 00h14m19.5908s -30d23m31.0272s (ICRS)',
-                                             '3.5816283341 -30.3919519949 (deg)')
-        assert label_mouseover.row1_unreliable
-        assert label_mouseover.row2_unreliable
-        assert label_mouseover.row3_unreliable
-
-        # Back to reference image
-        label_mouseover._viewer_mouse_event(self.viewer,
-                                            {'event': 'keydown', 'key': 'b',
-                                             'domain': {'x': 0, 'y': 0}})
-        self.viewer.on_mouse_or_key_event({'event': 'keydown', 'key': 'b',
-                                           'domain': {'x': 0, 'y': 0}})
-        assert label_mouseover.as_text() == ('Pixel x=00.0 y=00.0 Value +1.00000e+00 electron / s',
-                                             'World 00h14m19.5882s -30d23m31.0135s (ICRS)',
-                                             '3.5816174030 -30.3919481838 (deg)')
+        xy = self.viewer._get_real_xy(self.imviz.app.data_collection[0], 0, 0, reverse=True)
+        self.viewer.blink_once()
+        label_mouseover._viewer_mouse_event(
+            self.viewer, {'event': 'mousemove', 'domain': {'x': xy[0], 'y': xy[1]}})
+        assert label_mouseover.as_text()[0] in (
+            'Pixel x=00.0 y=00.0 Value +1.00000e+00 electron / s',
+            'Pixel x=-0.0 y=00.0 Value +1.00000e+00 electron / s',
+            'Pixel x=00.0 y=-0.0 Value +1.00000e+00 electron / s',
+            'Pixel x=-0.0 y=-0.0 Value +1.00000e+00 electron / s'
+        )
+        assert label_mouseover.as_text()[1:] == ('World 00h14m19.6141s -30d23m31.4091s (ICRS)',
+                                                 '3.5817255823 -30.3920580740 (deg)')
         assert not label_mouseover.row1_unreliable
         assert not label_mouseover.row2_unreliable
         assert not label_mouseover.row3_unreliable
 
-        # Still reference image but outside its own bounds.
-        label_mouseover._viewer_mouse_event(self.viewer,
-                                            {'event': 'mousemove', 'domain': {'x': 10, 'y': 3}})
-        assert label_mouseover.as_text() == ('Pixel x=10.0 y=03.0',
-                                             'World 00h14m19.6291s -30d23m30.9692s (ICRS)',
-                                             '3.5817877198 -30.3919358920 (deg)')
-        assert not label_mouseover.row1_unreliable
-        assert label_mouseover.row2_unreliable
-        assert label_mouseover.row3_unreliable
-
         # Regression test for https://github.com/spacetelescope/jdaviz/issues/2079 to
         # make sure this does not crash.
         viewer2 = self.imviz.create_image_viewer(viewer_name='second')
         viewer2.state.reset_limits()
 
+
+class TestLink_GWCS_GWCS(BaseImviz_GWCS_GWCS):
+
     def test_pixel_linking(self):
         self.imviz.link_data(link_type='pixels')
 
         # Check the coordinates display: Last loaded is on top.
         label_mouseover = self.imviz.app.session.application._tools['g-coords-info']
         label_mouseover._viewer_mouse_event(self.viewer,
                                             {'event': 'mousemove', 'domain': {'x': -1, 'y': -1}})
@@ -358,16 +282,17 @@
                                              '3.5815955408 -30.3919405616 (deg)')
         assert not label_mouseover.row1_unreliable
         assert label_mouseover.row2_unreliable
         assert label_mouseover.row3_unreliable
 
 
 def test_imviz_no_data(imviz_helper):
-    with pytest.raises(ValueError, match='No valid reference data'):
-        get_reference_image_data(imviz_helper.app)
+    refdata, iref = get_reference_image_data(imviz_helper.app)
+    assert refdata is None
+    assert iref == -1
 
-    imviz_helper.link_data(error_on_fail=True)  # Just no-op, do not crash
+    imviz_helper.link_data()  # Just no-op, do not crash
     links = imviz_helper.app.data_collection.external_links
     assert len(links) == 0
 
     with pytest.raises(ValueError, match='No reference data for link look-up'):
         imviz_helper.default_viewer._obj.get_link_type('foo')
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_parser.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,16 +262,18 @@
         assert isinstance(subsets['Subset 1'], CirclePixelRegion)
         assert isinstance(subsets['Subset 2'], RectanglePixelRegion)
 
         # Test simple aperture photometry plugin.
         phot_plugin = imviz_helper.app.get_tray_item_from_name('imviz-aper-phot-simple')
         phot_plugin.data_selected = 'contents[DATA]'
         phot_plugin.aperture_selected = 'Subset 1'
+        assert phot_plugin.aperture.selected_validity.get('is_aperture')
         assert_allclose(phot_plugin.background_value, 0)
         phot_plugin.background_selected = 'Subset 2'
+        assert phot_plugin.aperture.selected_validity.get('is_aperture')
         assert_allclose(phot_plugin.background_value, 0.1741226315498352)  # Subset 2 median
         # NOTE: jwst.datamodels.find_fits_keyword("PHOTMJSR")
         phot_plugin.counts_factor = (data.meta['photometry']['conversion_megajanskys'] /
                                      data.meta['exposure']['exposure_time'])
         assert_allclose(phot_plugin.counts_factor, 0.0036385915646798953)
         assert_allclose(phot_plugin.flux_scaling, 0.003631)
         phot_plugin.vue_do_aper_phot()
@@ -392,14 +394,15 @@
         # Test simple aperture photometry plugin.
         imviz_helper._apply_interactive_region('bqplot:ellipse',
                                                (1465, 2541),
                                                (1512, 2611))  # Galaxy
         phot_plugin = imviz_helper.app.get_tray_item_from_name('imviz-aper-phot-simple')
         phot_plugin.data_selected = 'contents[SCI,1]'
         phot_plugin.aperture_selected = 'Subset 1'
+        assert phot_plugin.aperture.selected_validity.get('is_aperture')
         phot_plugin.background_value = 0.0014  # Manual entry: Median on whole array
         assert_allclose(phot_plugin.pixel_area, 0.0025)  # Not used but still auto-populated
         phot_plugin.vue_do_aper_phot()
         tbl = imviz_helper.get_aperture_photometry_results()
         assert_quantity_allclose(tbl[0]['xcenter'], 1488.5 * u.pix, atol=2 * u.pix)
         assert_quantity_allclose(tbl[0]['ycenter'], 2576 * u.pix, atol=2 * u.pix)
         sky = tbl[0]['sky_center']
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_parser_asdf.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_parser_asdf.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_parser_roman.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_parser_roman.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_regions.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_regions.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_simple_aper_phot.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_simple_aper_phot.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,17 @@
     _curve_of_growth, _radial_profile)
 from jdaviz.configs.imviz.tests.utils import BaseImviz_WCS_WCS, BaseImviz_WCS_NoWCS
 
 
 class TestSimpleAperPhot(BaseImviz_WCS_WCS):
     def test_plugin_wcs_dithered(self):
         self.imviz.link_data(link_type='wcs')  # They are dithered by 1 pixel on X
-        self.imviz._apply_interactive_region('bqplot:truecircle', (0, 0), (9, 9))  # Draw a circle
+
+        reg = CirclePixelRegion(center=PixCoord(x=4.5, y=4.5), radius=4.5).to_sky(self.wcs_1)
+        self.imviz.load_regions(reg)
 
         phot_plugin = self.imviz.app.get_tray_item_from_name('imviz-aper-phot-simple')
 
         # Model fitting is already tested in astropy.
         # Here, we enable it just to make sure it does not crash.
         phot_plugin.fit_radial_profile = True
 
@@ -72,15 +74,15 @@
             'sum_aper_area', 'pixarea_tot', 'aperture_sum_counts', 'aperture_sum_counts_err',
             'counts_fac', 'aperture_sum_mag', 'flux_scaling', 'min', 'max', 'mean', 'median',
             'mode', 'std', 'mad_std', 'var', 'biweight_location', 'biweight_midvariance',
             'fwhm', 'semimajor_sigma', 'semiminor_sigma', 'orientation', 'eccentricity',
             'data_label', 'subset_label', 'timestamp']
         assert_array_equal(tbl['id'], [1, 2])
         assert_allclose(tbl['background'], 0)
-        assert_quantity_allclose(tbl['sum_aper_area'], [63.617251, 62.22684693104279] * (u.pix * u.pix))  # noqa
+        assert_quantity_allclose(tbl['sum_aper_area'], [63.617251, 62.22684693104279] * (u.pix * u.pix), rtol=1e-4)  # noqa
         assert_array_equal(tbl['pixarea_tot'], None)
         assert_array_equal(tbl['aperture_sum_counts'], None)
         assert_array_equal(tbl['aperture_sum_counts_err'], None)
         assert_array_equal(tbl['counts_fac'], None)
         assert_array_equal(tbl['aperture_sum_mag'], None)
         assert_array_equal(tbl['flux_scaling'], None)
         assert_allclose(tbl['min'], 1)
@@ -100,70 +102,77 @@
         assert_quantity_allclose(tbl['eccentricity'], 0)
         assert_array_equal(tbl['data_label'], ['has_wcs_1[SCI,1]', 'has_wcs_2[SCI,1]'])
         assert_array_equal(tbl['subset_label'], ['Subset 1', 'Subset 1'])
         assert tbl['timestamp'].scale == 'utc'
 
         # Sky is the same but xcenter different due to dithering.
         # The aperture sum is different too because mask is a little off limit in second image.
-        assert_quantity_allclose(tbl['xcenter'], [4.5, 5.5] * u.pix)
-        assert_quantity_allclose(tbl['ycenter'], 4.5 * u.pix)
+        assert_quantity_allclose(tbl['xcenter'], [4.5, 5.5] * u.pix, rtol=1e-4)
+        assert_quantity_allclose(tbl['ycenter'], 4.5 * u.pix, rtol=1e-4)
         sky = tbl['sky_center']
         assert_allclose(sky.ra.deg, 337.518943)
         assert_allclose(sky.dec.deg, -20.832083)
-        assert_allclose(tbl['sum'], [63.617251, 62.22684693104279])
+        assert_allclose(tbl['sum'], [63.617251, 62.22684693104279], rtol=1e-4)
 
         # Make sure it also works on an ellipse subset.
-        self.imviz._apply_interactive_region('bqplot:ellipse', (0, 0), (9, 4))
+        reg = EllipsePixelRegion(center=PixCoord(x=4.5, y=2.0), width=9.0, height=4.0).to_sky(self.wcs_1)  # noqa: E501
+        self.imviz.load_regions(reg)
+
         phot_plugin.dataset_selected = 'has_wcs_1[SCI,1]'
         phot_plugin.aperture_selected = 'Subset 2'
         phot_plugin.current_plot_type = 'Radial Profile'
         phot_plugin.vue_do_aper_phot()
         tbl = self.imviz.get_aperture_photometry_results()
         assert len(tbl) == 3  # New result is appended
         assert tbl[-1]['id'] == 3
-        assert_quantity_allclose(tbl[-1]['xcenter'], 4.5 * u.pix)
-        assert_quantity_allclose(tbl[-1]['ycenter'], 2 * u.pix)
+        assert_quantity_allclose(tbl[-1]['xcenter'], 4.5 * u.pix, rtol=1e-4)
+        assert_quantity_allclose(tbl[-1]['ycenter'], 2 * u.pix, rtol=1e-4)
         sky = tbl[-1]['sky_center']
-        assert_allclose(sky.ra.deg, 337.51894336144454)
-        assert_allclose(sky.dec.deg, -20.832777499255897)
-        assert_quantity_allclose(tbl[-1]['sum_aper_area'], 28.274334 * (u.pix * u.pix))
-        assert_allclose(tbl[-1]['sum'], 28.274334)
-        assert_allclose(tbl[-1]['mean'], 1)
+        assert_allclose(sky.ra.deg, 337.51894336144454, rtol=1e-4)
+        assert_allclose(sky.dec.deg, -20.832777499255897, rtol=1e-4)
+        assert_quantity_allclose(tbl[-1]['sum_aper_area'], 28.274334 * (u.pix * u.pix), rtol=1e-4)
+        assert_allclose(tbl[-1]['sum'], 28.274334, rtol=1e-4)
+        assert_allclose(tbl[-1]['mean'], 1, rtol=1e-4)
         assert tbl[-1]['data_label'] == 'has_wcs_1[SCI,1]'
         assert tbl[-1]['subset_label'] == 'Subset 2'
 
         # Make sure it also works on a rectangle subset.
         # We also subtract off background from itself here.
-        self.imviz._apply_interactive_region('bqplot:rectangle', (0, 0), (9, 9))
+        reg = RectanglePixelRegion(center=PixCoord(x=4.5, y=4.5), width=9, height=9).to_sky(self.wcs_1)  # noqa: E501
+        self.imviz.load_regions(reg)
+
         phot_plugin.dataset_selected = 'has_wcs_1[SCI,1]'
         phot_plugin.aperture_selected = 'Subset 3'
         phot_plugin.background_selected = 'Subset 3'
         assert_allclose(phot_plugin.background_value, 1)
         phot_plugin.vue_do_aper_phot()
         tbl = self.imviz.get_aperture_photometry_results()
         assert len(tbl) == 4  # New result is appended
         assert tbl[-1]['id'] == 4
         assert_quantity_allclose(tbl[-1]['xcenter'], 4.5 * u.pix)
         assert_quantity_allclose(tbl[-1]['ycenter'], 4.5 * u.pix)
         sky = tbl[-1]['sky_center']
-        assert_allclose(sky.ra.deg, 337.51894336144454)
-        assert_allclose(sky.dec.deg, -20.832083)
+        assert_allclose(sky.ra.deg, 337.51894336144454, rtol=1e-4)
+        assert_allclose(sky.dec.deg, -20.832083, rtol=1e-4)
         assert_quantity_allclose(tbl[-1]['sum_aper_area'], 81 * (u.pix * u.pix))
         assert_allclose(tbl[-1]['sum'], 0)
         assert_allclose(tbl[-1]['mean'], 0)
         assert tbl[-1]['data_label'] == 'has_wcs_1[SCI,1]'
         assert tbl[-1]['subset_label'] == 'Subset 3'
 
         # Make sure background auto-updates.
         phot_plugin.background_selected = 'Manual'
         assert_allclose(phot_plugin.background_value, 1)  # Keeps last value
         phot_plugin.background_selected = 'Subset 1'
         assert_allclose(phot_plugin.background_value, 1)
-        self.imviz.load_data(np.ones((10, 10)) + 1, data_label='twos')
-        phot_plugin.dataset_selected = 'twos'
+
+        hdu3 = fits.ImageHDU(np.ones((10, 10)) + 1, name='SCI')
+        hdu3.header.update(self.wcs_2.to_header())
+        self.imviz.load_data(hdu3, data_label='twos')
+        phot_plugin.dataset_selected = 'twos[SCI,1]'
         assert_allclose(phot_plugin.background_value, 2)  # Recalculate based on new Data
 
         # Curve of growth
         phot_plugin.current_plot_type = 'Curve of Growth'
         phot_plugin.vue_do_aper_phot()
         assert phot_plugin.plot.figure.title == 'Curve of growth from aperture center'
 
@@ -257,41 +266,33 @@
         fn_1 = get_pkg_data_filename('data/gauss100_fits_wcs.fits')
         imviz_helper.load_data(fn_1)
         # Different pixel scale
         imviz_helper.load_data(get_pkg_data_filename('data/gauss100_fits_wcs_block_reduced.fits'))
         # Different pixel scale + rotated
         imviz_helper.load_data(get_pkg_data_filename('data/gauss100_fits_wcs_block_reduced_rotated.fits'))  # noqa: E501
 
-        # Reference image again but without any WCS
-        data = fits.getdata(fn_1, ext=0)
-        imviz_helper.load_data(data, data_label='no_wcs')
-
         # Link them by WCS
         imviz_helper.link_data(link_type='wcs')
+        w = imviz_helper.app.data_collection[0].coords
 
         # Regions to be used for aperture photometry
-        regions = []
-        positions = [(145.1, 168.3), (48.3, 200.3)]
-        for x, y in positions:
-            regions.append(CirclePixelRegion(center=PixCoord(x=x, y=y), radius=5))
-        regions += [
-            EllipsePixelRegion(center=PixCoord(x=84.7, y=224.1), width=23, height=9,
-                               angle=2.356 * u.rad),
-            RectanglePixelRegion(center=PixCoord(x=229, y=152), width=17, height=7)]
-        imviz_helper.load_regions(regions)
+        imviz_helper.load_regions([
+            CirclePixelRegion(center=PixCoord(x=145.1, y=168.3), radius=5).to_sky(w),
+            CirclePixelRegion(center=PixCoord(x=48.3, y=200.3), radius=5).to_sky(w),
+            EllipsePixelRegion(center=PixCoord(x=84.7, y=224.1), width=23, height=9, angle=2.356 * u.rad).to_sky(w),  # noqa: E501
+            RectanglePixelRegion(center=PixCoord(x=229, y=152), width=17, height=7).to_sky(w)])
 
         self.imviz = imviz_helper
         self.viewer = imviz_helper.default_viewer._obj
         self.phot_plugin = imviz_helper.plugins["Aperture Photometry"]._obj
 
     @pytest.mark.parametrize(('data_label', 'local_bkg'), [
         ('gauss100_fits_wcs[PRIMARY,1]', 5.0),
         ('gauss100_fits_wcs_block_reduced[PRIMARY,1]', 20.0),
-        ('gauss100_fits_wcs_block_reduced_rotated[PRIMARY,1]', 20.0),
-        ('no_wcs', 5.0)])
+        ('gauss100_fits_wcs_block_reduced_rotated[PRIMARY,1]', 20.0)])
     @pytest.mark.parametrize(('subset_label', 'expected_sum'), [
         ('Subset 1', 738.8803424408962),
         ('Subset 2', 857.5194857987592),
         ('Subset 3', 472.17364321556005),
         ('Subset 4', 837.0023608207703)])
     def test_aperphot(self, data_label, local_bkg, subset_label, expected_sum):
         """All data should give similar result for the same Subset."""
@@ -304,16 +305,16 @@
 
         # Imperfect down-sampling and imperfect apertures, so 10% is good enough.
         assert_allclose(tbl['sum'][-1], expected_sum, rtol=0.1)
 
     @pytest.mark.parametrize(('data_label', 'fac'), [
         ('gauss100_fits_wcs[PRIMARY,1]', 1),
         ('gauss100_fits_wcs_block_reduced[PRIMARY,1]', 4),
-        ('gauss100_fits_wcs_block_reduced_rotated[PRIMARY,1]', 4),
-        ('no_wcs', 1)])
+        ('gauss100_fits_wcs_block_reduced_rotated[PRIMARY,1]', 4)
+    ])
     @pytest.mark.parametrize(('bg_label', 'expected_bg'), [
         ('Subset 2', 12.269274711608887),
         ('Subset 3', 7.935906410217285),
         ('Subset 4', 11.120951652526855)])
     def test_sky_background(self, data_label, fac, bg_label, expected_bg):
         """All background (median) should give similar result for the same Subset.
         Down-sampled data has higher factor due to flux conservation.
@@ -335,46 +336,49 @@
     imviz_helper.load_data(gauss4, data_label='four_gaussians')
     imviz_helper.load_data(ones, data_label='ones')
 
     phot_plugin = imviz_helper.app.get_tray_item_from_name('imviz-aper-phot-simple')
     phot_plugin.dataset_selected = 'ones'
 
     # Mark an object of interest
-    # CirclePixelRegion(center=PixCoord(x=150, y=25), radius=7)
-    imviz_helper._apply_interactive_region('bqplot:truecircle', (143, 18), (157, 32))
-
+    circle_1 = CirclePixelRegion(center=PixCoord(x=150, y=25), radius=7)
     # Load annulus (this used to be part of the plugin but no longer)
     annulus_1 = CircleAnnulusPixelRegion(
         PixCoord(x=150, y=25), inner_radius=7, outer_radius=17)
-    imviz_helper.load_regions([annulus_1])
+    imviz_helper.load_regions([circle_1, annulus_1])
 
     phot_plugin.aperture_selected = 'Subset 1'
     phot_plugin.background_selected = 'Subset 2'
 
     # Check annulus for ones
     assert_allclose(phot_plugin.background_value, 1)
 
     # Switch data
     phot_plugin.dataset_selected = 'four_gaussians'
     assert_allclose(phot_plugin.background_value, 5.745596129482831)  # Changed
 
     # Draw ellipse on another object
-    # EllipsePixelRegion(center=PixCoord(x=20.5, y=37.5), width=41, height=15)
-    imviz_helper._apply_interactive_region('bqplot:ellipse', (0, 30), (41, 45))
-
+    ellipse_1 = EllipsePixelRegion(center=PixCoord(x=20.5, y=37.5), width=41, height=15)
     # Load annulus (this used to be part of the plugin but no longer)
     annulus_2 = CircleAnnulusPixelRegion(
         PixCoord(x=20.5, y=37.5), inner_radius=20.5, outer_radius=30.5)
-    imviz_helper.load_regions([annulus_2])
+    imviz_helper.load_regions([ellipse_1, annulus_2])
 
-    # Subset 4 (annulus) should be available for the background but not the aperture
-    assert 'Subset 4' not in phot_plugin.aperture.choices
+    # Subset 4 (annulus) should be available in both sets of choices, but invalid for selection as
+    # aperture
+    assert 'Subset 4' in phot_plugin.aperture.choices
     assert 'Subset 4' in phot_plugin.background.choices
 
+    phot_plugin.aperture_selected = 'Subset 4'
+    assert not phot_plugin.aperture.selected_validity.get('is_aperture', True)
+    with pytest.raises(ValueError, match="Selected aperture is not valid"):
+        phot_plugin.calculate_photometry()
+
     phot_plugin.aperture_selected = 'Subset 3'
+    assert phot_plugin.aperture.selected_validity.get('is_aperture', False)
     phot_plugin.background_selected = 'Subset 4'
 
     # Check new annulus for four_gaussians
     assert_allclose(phot_plugin.background_value, 5.13918435824334)  # Changed
 
     # Switch to manual, should not change
     phot_plugin.background_selected = 'Manual'
@@ -387,18 +391,18 @@
     # Switch back to annulus, should be same as before in same mode
     phot_plugin.background_selected = 'Subset 4'
     assert_allclose(phot_plugin.background_value, 5.13918435824334)
 
     # Edit the annulus and make sure background updates
     subset_plugin = imviz_helper.plugins["Subset Tools"]._obj
     subset_plugin.subset_selected = "Subset 4"
-    subset_plugin._set_value_in_subset_definition(0, "X Center", "value", 25.5)
-    subset_plugin._set_value_in_subset_definition(0, "Y Center", "value", 42.5)
-    subset_plugin._set_value_in_subset_definition(0, "Inner radius", "value", 40)
-    subset_plugin._set_value_in_subset_definition(0, "Outer radius", "value", 45)
+    subset_plugin._set_value_in_subset_definition(0, "X Center (pixels)", "value", 25.5)
+    subset_plugin._set_value_in_subset_definition(0, "Y Center (pixels)", "value", 42.5)
+    subset_plugin._set_value_in_subset_definition(0, "Inner Radius (pixels)", "value", 40)
+    subset_plugin._set_value_in_subset_definition(0, "Outer Radius (pixels)", "value", 45)
     subset_plugin.vue_update_subset()
     assert_allclose(phot_plugin.background_value, 4.89189)
 
 
 # NOTE: Extracting the cutout for radial profile is aperture
 #       shape agnostic, so we use ellipse as representative case.
 # NOTE: This test only tests the radial profile algorithm and does
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_tools.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import numpy as np
+import pytest
+from astropy.coordinates import SkyCoord
+from astropy.nddata import NDData
 from numpy.testing import assert_allclose
-from regions import RectanglePixelRegion
 
-from jdaviz.configs.imviz.tests.utils import BaseImviz_WCS_WCS
+from jdaviz.configs.imviz.tests.utils import BaseImviz_WCS_WCS, create_example_gwcs
 
 
 class TestPanZoomTools(BaseImviz_WCS_WCS):
     def test_panzoom_tools(self):
         v = self.imviz.default_viewer._obj
         v2 = self.imviz.create_image_viewer()
         self.imviz.app.add_data_to_viewer('imviz-1', 'has_wcs_1[SCI,1]')
@@ -61,49 +63,52 @@
         t_linkedpan.on_click({'event': 'click', 'domain': {'x': 2, 'y': 2}})
         # make sure both viewers moved to the new center
         assert_allclose((v.state.x_min, v.state.x_max, v.state.y_min, v.state.y_max), (-1.5, 5.5, -1.5, 5.5))  # noqa
         assert_allclose((v2.state.x_min, v2.state.x_max, v2.state.y_min, v2.state.y_max), (-1.5, 5.5, -1.5, 5.5))  # noqa
         t_linkedpan.deactivate()
 
 
-# We use a new test class to avoid a dirty state from previous test.
-class TestSinglePixelRegion(BaseImviz_WCS_WCS):
-    def test_singlepixelregion(self):
-        self.imviz.link_data(link_type='wcs')
-
-        t = self.imviz.default_viewer._obj.toolbar.tools['jdaviz:singlepixelregion']
-        t.activate()
-
-        # Create a region while viewing reference data.
-        t.on_mouse_event({'event': 'click', 'altKey': False, 'domain': {'x': 1, 'y': 2}})
-        regions = self.imviz.get_interactive_regions()
-        assert len(regions) == 1
-        reg = regions['Subset 1']
-        assert (isinstance(reg, RectanglePixelRegion) and reg.center.x == 1 and reg.center.y == 2
-                and reg.width == 1 and reg.height == 1)
-
-        # Clicking again will move the region, not creating a new one.
-        t.on_mouse_event({'event': 'click', 'altKey': False, 'domain': {'x': 2, 'y': 3}})
-        regions = self.imviz.get_interactive_regions()
-        assert len(regions) == 1
-        reg = regions['Subset 1']
-        assert (isinstance(reg, RectanglePixelRegion) and reg.center.x == 2 and reg.center.y == 3
-                and reg.width == 1 and reg.height == 1)
-
-        # Create a new region while viewing dithered data.
-        # Region will still be w.r.t. reference data, that is, x and y from domain stay the same.
-        self.imviz.default_viewer.blink_once()
-        t.on_mouse_event({'event': 'click', 'altKey': True, 'domain': {'x': 3, 'y': 4}})
-        regions = self.imviz.get_interactive_regions()
-        assert len(regions) == 2
-        reg = regions['Subset 2']
-        assert (isinstance(reg, RectanglePixelRegion) and reg.center.x == 3 and reg.center.y == 4
-                and reg.width == 1 and reg.height == 1)
-
-        t.deactivate()
+@pytest.mark.parametrize("link_type", ["Pixels", "WCS"])
+def test_panzoom_click_center_linking(imviz_helper, link_type):
+    """https://github.com/spacetelescope/jdaviz/issues/2749"""
+    v = imviz_helper.default_viewer._obj
+
+    # Since we are not really displaying, need this to test pan/zoom.
+    v.shape = (100, 100)
+    v.state._set_axes_aspect_ratio(1)
+
+    arr_big = np.ones((40, 30), dtype=int)
+    w_big = create_example_gwcs(arr_big.shape)
+    arr_small = np.ones((20, 15), dtype=int)
+    w_small = create_example_gwcs(arr_small.shape)
+
+    imviz_helper.load_data(NDData(arr_big, wcs=w_big), data_label="big")
+    imviz_helper.load_data(NDData(arr_small, wcs=w_small), data_label="small")
+
+    lc_plugin = imviz_helper.plugins['Orientation']
+    lc_plugin.link_type = link_type
+
+    coo = SkyCoord(ra=197.89262754541807, dec=-1.3644568140486624, unit="deg")
+
+    if link_type == "WCS":
+        mouseover_loc = v.state.reference_data.coords.world_to_pixel(coo)
+    else:  # Pixels
+        mouseover_loc = w_small.world_to_pixel(coo)
+
+    t = v.toolbar.tools['jdaviz:imagepanzoom']
+    t.activate()
+    t.on_click({'event': 'click', 'domain': {'x': mouseover_loc[0], 'y': mouseover_loc[1]}})
+    t.deactivate()
+
+    # We want to make sure click centers viewer to where it is supposed to be.
+    cur_cen = v._get_center_skycoord()
+    v.center_on(coo)
+    real_cen = v._get_center_skycoord()
+    assert_allclose(cur_cen.ra.deg, real_cen.ra.deg)
+    assert_allclose(cur_cen.dec.deg, real_cen.dec.deg)
 
 
 def test_blink(imviz_helper):
     viewer = imviz_helper.default_viewer._obj
 
     for i in range(3):
         imviz_helper.load_data(np.zeros((2, 2)) + i, data_label=f'image_{i}')
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_viewer_tools.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_viewer_tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/tests/test_viewers.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/tests/test_viewers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/imviz/tests/utils.py` & `jdaviz-3.9.0/jdaviz/configs/imviz/tests/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,18 +134,16 @@
         pipeline = [(detector_frame, det2sky), (sky_frame, None)]
         w_gwcs = gwcs.WCS(pipeline)
         w_gwcs.bounding_box = ((0, 8), (0, 10)) * u.pix  # x, y
 
         # Load data into Imviz:
         # 1. Data with FITS WCS and unit.
         # 2. Data with GWCS (rotated w.r.t. FITS WCS) and no unit.
-        # 3. Data without WCS nor unit.
         imviz_helper.load_data(NDData(arr, wcs=w_fits, unit='electron/s'), data_label='fits_wcs')
         imviz_helper.load_data(NDData(arr, wcs=w_gwcs), data_label='gwcs')
-        imviz_helper.load_data(arr, data_label='no_wcs')
 
         self.wcs_1 = w_fits
         self.wcs_2 = w_gwcs
         self.imviz = imviz_helper
         self.viewer = imviz_helper.default_viewer._obj
 
         # Since we are not really displaying, need this to test zoom.
@@ -234,15 +232,15 @@
     sky_frame = cf.CelestialFrame(reference_frame=ICRS(), name='icrs', unit=(u.deg, u.deg))
 
     pipeline = [(detector_frame, det2sky), (sky_frame, None)]
 
     return gwcs_wcs.WCS(pipeline)
 
 
-def create_wfi_image_model(image_shape, **kwargs):
+def create_wfi_image_model(image_shape=(20, 10), **kwargs):
     """
     Create a dummy Roman WFI ImageModel instance with valid values
     for attributes required by the schema.
 
     Requires roman_datamodels >= 0.14.2
 
     Parameters
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/mosviz/helper.py` & `jdaviz-3.9.0/jdaviz/configs/mosviz/helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/mosviz/mosviz.ipynb` & `jdaviz-3.9.0/jdaviz/configs/mosviz/mosviz.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/mosviz/mosviz.yaml` & `jdaviz-3.9.0/jdaviz/configs/mosviz/mosviz.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   - g-subset-plugin
   - g-markers
   - g-gaussian-smooth
   - g-slit-overlay
   - g-model-fitting
   - g-line-list
   - specviz-line-analysis
-  - g-export-plot
+  - export
 viewer_area:
   - container: col
     children:
     - container: col
       children:
       - container: row
         children:
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/mosviz/plugins/parsers.py` & `jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/mosviz/plugins/row_lock/row_lock.py` & `jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/row_lock/row_lock.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.py` & `jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/mosviz/plugins/slit_overlay/tests/test_slit_overlay.py` & `jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/slit_overlay/tests/test_slit_overlay.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/mosviz/plugins/tools.py` & `jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/mosviz/plugins/viewers.py` & `jdaviz-3.9.0/jdaviz/configs/mosviz/plugins/viewers.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
                     ['jdaviz:homezoom', 'jdaviz:prevzoom'],
                     ['jdaviz:boxzoom'],
                     ['jdaviz:panzoom'],
                     ['jdaviz:sidebar_plot', 'jdaviz:sidebar_export']
                 ]
 
     default_class = None
+    _state_cls = FreezableBqplotImageViewerState
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.init_astrowidgets_api()
         self._subscribe_to_layers_update()
 
         self.state.show_axes = False  # Axes are wrong anyway
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/mosviz/tests/test_data_loading.py` & `jdaviz-3.9.0/jdaviz/configs/mosviz/tests/test_data_loading.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/mosviz/tests/test_helper.py` & `jdaviz-3.9.0/jdaviz/configs/mosviz/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/mosviz/tests/test_parsers.py` & `jdaviz-3.9.0/jdaviz/configs/mosviz/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/mosviz/tests/test_source_identifier_extract.py` & `jdaviz-3.9.0/jdaviz/configs/mosviz/tests/test_source_identifier_extract.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/mosviz/tests/test_tools.py` & `jdaviz-3.9.0/jdaviz/configs/mosviz/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/specviz/helper.py` & `jdaviz-3.9.0/jdaviz/configs/specviz/helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,25 +217,25 @@
         if min_val is not None:
             # If SpectralRegion, set limits to region's lower and upper bounds
             if isinstance(min_val, SpectralRegion):
                 return self._set_scale(scale, axis, min_val.lower, min_val.upper)
             # If user's value has a unit, convert it to the current axis' units
             elif isinstance(min_val, u.Quantity):
                 # Convert user's value to axis' units
-                min_val = min_val.to(axis.unit).value
+                min_val = min_val.to_value(axis.unit)
             # If auto, set to min axis wavelength value
             elif min_val == "auto":
                 min_val = min(axis).value
 
             scale.min = float(min_val)
         if max_val is not None:
             # If user's value has a unit, convert it to the current axis' units
             if isinstance(max_val, u.Quantity):
                 # Convert user's value to axis' units
-                max_val = max_val.to(axis.unit).value
+                max_val = max_val.to_value(axis.unit)
             # If auto, set to max axis wavelength value
             elif max_val == "auto":
                 max_val = max(axis).value
 
             scale.max = float(max_val)
 
     def autoscale_x(self):
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.py` & `jdaviz-3.9.0/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 import os
-import warnings
+import logging
 
 import numpy as np
 from glue.core.message import (SubsetDeleteMessage,
                                SubsetUpdateMessage)
 from glue_jupyter.common.toolbar_vuetify import read_icon
 from traitlets import Bool, List, Float, Unicode, observe
 from astropy import units as u
 from specutils import analysis, Spectrum1D
-from specutils.manipulation import extract_region
 
-from jdaviz.core.custom_traitlets import FloatHandleEmpty
 from jdaviz.core.events import (AddDataMessage,
                                 RemoveDataMessage,
                                 SpectralMarksChangedMessage,
                                 LineIdentifyMessage,
                                 RedshiftMessage,
                                 GlobalDisplayUnitChanged,
                                 SnackbarMessage)
-from jdaviz.core.marks import (LineAnalysisContinuum,
-                               LineAnalysisContinuumCenter,
-                               LineAnalysisContinuumLeft,
-                               LineAnalysisContinuumRight,
-                               ShadowLine)
 from jdaviz.core.registries import tray_registry
 from jdaviz.core.template_mixin import (PluginTemplateMixin,
                                         DatasetSelectMixin,
                                         SpectralSubsetSelectMixin,
                                         DatasetSpectralSubsetValidMixin,
                                         SubsetSelect,
+                                        SpectralContinuumMixin,
                                         SPATIAL_DEFAULT_TEXT,
-                                        skip_if_no_updates_since_last_active)
+                                        skip_if_no_updates_since_last_active,
+                                        with_spinner)
 from jdaviz.core.user_api import PluginUserApi
 from jdaviz.core.tools import ICON_DIR
 
 
 __all__ = ['LineAnalysis']
 
 FUNCTIONS = {"Line Flux": analysis.line_flux,
@@ -66,15 +61,15 @@
     if getattr(quantity, 'uncertainty', None) is not None:
         coerced_quantity.uncertainty = quantity.uncertainty.to(coerced_unit_string)
     return coerced_quantity
 
 
 @tray_registry('specviz-line-analysis', label="Line Analysis", viewer_requirements='spectrum')
 class LineAnalysis(PluginTemplateMixin, DatasetSelectMixin, SpectralSubsetSelectMixin,
-                   DatasetSpectralSubsetValidMixin):
+                   DatasetSpectralSubsetValidMixin, SpectralContinuumMixin):
     """
     The Line Analysis plugin returns specutils analysis for a single spectral line.
     See the :ref:`Line Analysis Plugin Documentation <line-analysis>` for more details.
 
     Only the following attributes and methods are available through the
     :ref:`public plugin API <plugin-apis>`:
 
@@ -86,32 +81,28 @@
     * ``spatial_subset`` (:class:`~jdaviz.core.template_mixin.SubsetSelect`):
       Select which region's collapsed spectrum to analyze or ``Entire Cube``.
     * ``spectral_subset`` (:class:`~jdaviz.core.template_mixin.SubsetSelect`):
       Subset to use for the line, or ``Entire Spectrum``.
     * ``continuum`` (:class:`~jdaviz.core.template_mixin.SubsetSelect`):
       Subset to use for the continuum, or ``Surrounding`` to use a region surrounding the
       subset set in ``spectral_subset``.
-    * :attr:`width`:
+    * ```continuum_width``:
       Width, relative to the overall line spectral region, to fit the linear continuum
       (excluding the region containing the line). If 1, will use endpoints within line region
       only.
     * :meth:`get_results`
 
     """
     dialog = Bool(False).tag(sync=True)
     template_file = __file__, "line_analysis.vue"
     uses_active_status = Bool(True).tag(sync=True)
 
     spatial_subset_items = List().tag(sync=True)
     spatial_subset_selected = Unicode().tag(sync=True)
 
-    continuum_subset_items = List().tag(sync=True)
-    continuum_subset_selected = Unicode().tag(sync=True)
-
-    width = FloatHandleEmpty(3).tag(sync=True)
     results_computing = Bool(False).tag(sync=True)
     results = List().tag(sync=True)
     results_centroid = Float().tag(sync=True)  # stored in AA units
     line_items = List([]).tag(sync=True)
     sync_identify = Bool(True).tag(sync=True)
     sync_identify_icon_enabled = Unicode(read_icon(os.path.join(ICON_DIR, 'line_select.svg'), 'svg+xml')).tag(sync=True)  # noqa
     sync_identify_icon_disabled = Unicode(read_icon(os.path.join(ICON_DIR, 'line_select_disabled.svg'), 'svg+xml')).tag(sync=True)  # noqa
@@ -121,25 +112,22 @@
 
     def __init__(self, *args, **kwargs):
 
         super().__init__(**kwargs)
 
         self.update_results(None)
 
-        self.continuum = SubsetSelect(self,
-                                      'continuum_subset_items',
-                                      'continuum_subset_selected',
-                                      default_text='Surrounding',
-                                      filters=['is_spectral'])
-
         # when accessing the selected data, access the spectrum-viewer version
         self.dataset._viewers = [self._default_spectrum_viewer_reference_name]
         # require entries to be in spectrum-viewer (not other cubeviz images, etc)
         self.dataset.add_filter('layer_in_spectrum_viewer')
 
+        # continuum selection is mandatory for line-analysis
+        self._continuum_remove_none_option()
+
         if self.app.state.settings.get("configuration") == "cubeviz":
             self.spatial_subset = SubsetSelect(self,
                                                'spatial_subset_items',
                                                'spatial_subset_selected',
                                                default_text=SPATIAL_DEFAULT_TEXT,
                                                filters=['is_spatial'])
         else:
@@ -163,18 +151,31 @@
 
     @property
     def _default_spectrum_viewer_reference_name(self):
         return getattr(
             self.app._jdaviz_helper, '_default_spectrum_viewer_reference_name', 'spectrum-viewer'
         )
 
+    # backwards compatibility for width (replace with user API deprecation)
+    @property
+    def width(self):
+        logging.warning(f"DeprecationWarning: width was replaced by continuum_width in 3.9 and will be removed in a future release")  # noqa
+        return self.continuum_width
+
+    @width.setter
+    def width(self, width):
+        logging.warning("DeprecationWarning: width was replaced by continuum_width in 3.9 and will be removed in a future release")  # noqa
+        self.continuum_width = width
+
     @property
     def user_api(self):
+        # deprecated: width was replaced with continuum_width in 3.9 so should be removed from the
+        # user API and the property and setter above as soon as 3.11.
         return PluginUserApi(self, expose=('dataset', 'spatial_subset', 'spectral_subset',
-                                           'continuum', 'width', 'get_results'))
+                                           'continuum', 'width', 'continuum_width', 'get_results'))
 
     def _on_viewer_data_changed(self, msg):
         viewer_id = self.app._viewer_item_by_reference(
             self._default_spectrum_viewer_reference_name
         ).get('id')
         if msg is None or msg.viewer_id != viewer_id or msg.data is None:
             return
@@ -220,60 +221,25 @@
         self._calculate_statistics(msg)
 
     @observe('is_active')
     def _is_active_changed(self, msg):
         if self.disabled_msg:
             return
 
-        for pos, mark in self.marks.items():
+        for pos, mark in self.continuum_marks.items():
             mark.visible = self.is_active
         self._calculate_statistics(msg)
 
-    @property
-    def marks(self):
-        marks = {}
-        viewer = self.app.get_viewer(self._default_spectrum_viewer_reference_name)
-        if viewer is None:
-            return {}
-        for mark in viewer.figure.marks:
-            if isinstance(mark, LineAnalysisContinuum):
-                # NOTE: we don't use isinstance anymore because of nested inheritance
-                if mark.__class__.__name__ == 'LineAnalysisContinuumLeft':
-                    marks['left'] = mark
-                elif mark.__class__.__name__ == 'LineAnalysisContinuumCenter':
-                    marks['center'] = mark
-                elif mark.__class__.__name__ == 'LineAnalysisContinuumRight':
-                    marks['right'] = mark
-
-        if not len(marks):
-            if not viewer.state.reference_data:
-                # we don't have data yet for scales, defer initializing
-                return {}
-            # then haven't been initialized yet, so initialize with empty
-            # marks that will be populated once the first analysis is done.
-            marks = {'left': LineAnalysisContinuumLeft(viewer, visible=self.is_active),
-                     'center': LineAnalysisContinuumCenter(viewer, visible=self.is_active),
-                     'right': LineAnalysisContinuumRight(viewer, visible=self.is_active)}
-            shadows = [ShadowLine(mark, shadow_width=2) for mark in marks.values()]
-            # NOTE: += won't trigger the figure to notice new marks
-            viewer.figure.marks = viewer.figure.marks + shadows + list(marks.values())
-
-        return marks
-
-    def update_results(self, results=None, mark_x={}, mark_y={}):
-        for pos, mark in self.marks.items():
-            mark.update_xy(mark_x.get(pos, []), mark_y.get(pos, []))
-
+    def update_results(self, results=None):
         if results is None:
             self.results = [{'function': function, 'result': ''} for function in FUNCTIONS]
+            self._update_continuum_marks()
         else:
             self.results = results
 
-        self.results_computing = False
-
     def get_results(self):
         # user-facing API call to force updating and retrieving results, even if the plugin
         # is closed
 
         if not self.spectral_subset_valid:
             valid, spec_range, subset_range = self._check_dataset_spectral_subset_valid(return_ranges=True)  # noqa
             raise ValueError(f"spectral subset '{self.spectral_subset.selected}' {subset_range} is outside data range of '{self.dataset.selected}' {spec_range}")  # noqa
@@ -293,156 +259,57 @@
         if self.sync_identify or not self.selected_line:
             # then we should follow the identified line, either because of sync
             # or because nothing has been selected yet.
             # if results aren't available yet, then we'll wait until they are
             # in which case we'll default to the identified line
             self.selected_line = self.identified_line
 
-    @observe("spatial_subset_selected", "spectral_subset_selected", "dataset_selected",
-             "continuum_subset_selected", "width")
+    @observe("dataset_selected", "spatial_subset_selected", "spectral_subset_selected",
+             "continuum_subset_selected", "continuum_width")
     @skip_if_no_updates_since_last_active()
+    @with_spinner('results_computing')
     def _calculate_statistics(self, msg={}):
         """
         Run the line analysis functions on the selected data/subset and
         display the results.
         """
-        if not hasattr(self, 'dataset') or self.app._jdaviz_helper is None or self.dataset_selected == '':  # noqa
+        if not hasattr(self, 'dataset') or self.app._jdaviz_helper is None:  # noqa
             # during initial init, this can trigger before the component is initialized
             return
+
         if self.disabled_msg != '':
             self.update_results(None)
             return
 
         # call directly since this observe may be triggered before the spectral_subset_valid
         # traitlet is updated
         if not self._check_dataset_spectral_subset_valid():
             # skip gracefully, if the user called from get_results, and error would be raised there
             self.update_results(None)
             return
 
-        # show spinner with overlay
-        self.results_computing = True
-        full_spectrum = self.dataset.selected_spectrum_for_spatial_subset(self.spatial_subset_selected,  # noqa
-                                                                          use_display_units=True)
-
-        if full_spectrum is None or self.width == "":
-            # this can happen DURING a unit conversion change
-            self.update_results(None)
-            return
-
-        spectral_axis = full_spectrum.spectral_axis
-        if spectral_axis.unit == u.pix:
-            # plugin should be disabled so not get this far, but can still get here
-            # before the disabled message is set
-            self.update_results(None)
-            return
-
-        if self.continuum_subset_selected == self.spectral_subset_selected:
-            # already raised a validation error in the UI
+        spectrum, continuum, spec_subtracted = self._get_continuum(self.dataset,
+                                                                   self.spatial_subset,
+                                                                   self.spectral_subset,
+                                                                   update_marks=True)
+        if spectrum is None:
             self.update_results(None)
             return
 
-        if self.spectral_subset_selected == "Entire Spectrum":
-            spectrum = full_spectrum
-        else:
-            sr = self.app.get_subsets(self.spectral_subset_selected,
-                                      simplify_spectral=True, use_display_units=True)
-            spectrum = extract_region(full_spectrum, sr, return_single_spectrum=True)
-            sr_lower = np.nanmin(spectrum.spectral_axis[spectrum.spectral_axis.value >= sr.lower.value])  # noqa
-            sr_upper = np.nanmax(spectrum.spectral_axis[spectrum.spectral_axis.value <= sr.upper.value])  # noqa
-
-        # compute continuum
-        if self.continuum_subset_selected == "Surrounding" and self.spectral_subset_selected == "Entire Spectrum": # noqa
-            # we know we'll just use the endpoints, so let's be efficient and not even
-            # try extracting from the region
-            continuum_mask = np.array([0, len(spectral_axis)-1])
-            mark_x = {'left': np.array([]),
-                      'center': np.array([min(spectral_axis.value), max(spectral_axis.value)]),
-                      'right': np.array([])}
-
-        elif self.continuum_subset_selected == "Surrounding":
-            # self.spectral_subset_selected != "Entire Spectrum"
-            if self.width > 10 or self.width < 1:
-                # DEV NOTE: if changing the limits, make sure to also update the form validation
-                # rules in line_analysis.vue
-                self.update_results(None)
-                return
-
-            spectral_region_width = sr_upper - sr_lower
-            # convert width from total relative width, to width per "side"
-            width = (self.width - 1) / 2
-            left, = np.where((spectral_axis < sr_lower) &
-                             (spectral_axis > sr_lower - spectral_region_width*width))
-            if not len(left):
-                # then no points matching the width are available outside the line region,
-                # so we'll default to the left-most point of the line region.
-                left, = np.where(spectral_axis == min(spectrum.spectral_axis))
-
-            right, = np.where((spectral_axis > sr_upper) &
-                              (spectral_axis < sr_upper + spectral_region_width*width))
-            if not len(right):
-                # then no points matching the width are available outside the line region,
-                # so we'll default to the right-most point of the line region.
-                right, = np.where(spectral_axis == max(spectrum.spectral_axis))
-
-            continuum_mask = np.concatenate((left, right))
-            mark_x = {'left': np.array([min(spectral_axis.value[continuum_mask]), sr_lower.value]),
-                      'center': np.array([sr_lower.value, sr_upper.value]),
-                      'right': np.array([sr_upper.value, max(spectral_axis.value[continuum_mask])])}
-
-        else:
-            # we'll access the mask of the continuum and then apply that to the spectrum.  For a
-            # spatially-collapsed spectrum in cubeviz, this will access the mask from the full
-            # cube, but still apply that to the spatially-collapsed spectrum.
-            continuum_mask = ~self._specviz_helper.get_data(
-                self.dataset.selected,
-                spectral_subset=self.continuum_subset_selected,
-                use_display_units=False).mask
-            spectral_axis_nanmasked = spectral_axis.value.copy()
-            spectral_axis_nanmasked[~continuum_mask] = np.nan
-            if self.spectral_subset_selected == "Entire Spectrum":
-                mark_x = {'left': spectral_axis_nanmasked,
-                          'center': spectral_axis.value,
-                          'right': []}
-            else:
-                mark_x = {'left': spectral_axis_nanmasked[spectral_axis.value < sr_lower.value],
-                          'right': spectral_axis_nanmasked[spectral_axis.value > sr_upper.value]}
-                # Center should extend (at least) across the line region between the full
-                # range defined by the continuum subset(s).
-                # OK for mark_x to be all NaNs.
-                with warnings.catch_warnings():
-                    warnings.simplefilter('ignore', category=RuntimeWarning)
-                    mark_x_min = np.nanmin(mark_x['left'])
-                    mark_x_max = np.nanmax(mark_x['right'])
-                left_min = np.nanmin([mark_x_min, sr_lower.value])
-                right_max = np.nanmax([mark_x_max, sr_upper.value])
-                mark_x['center'] = np.array([left_min, right_max])
-
-        continuum_x = spectral_axis[continuum_mask].value
-        min_x = min(spectral_axis.value)
-        continuum_y = full_spectrum.flux[continuum_mask].value
-        # DEV NOTE: could replace this with internal calls to the model fitting infrastructure
-        # to enable other model-types and to give visual feedback (by labeling the model
-        # as line_analysis:continuum, for example)
-        slope, intercept = np.polyfit(continuum_x-min_x, continuum_y, deg=1)
-        continuum = slope * (spectrum.spectral_axis.value-min_x) + intercept
-        mark_y = {k: slope * (v-min_x) + intercept for k, v in mark_x.items()}
-
         def _uncertainty(result):
             if getattr(result, 'uncertainty', None) is not None:
                 # we'll keep the uncertainty and result in the same unit (so
                 # we only have to show the unit at the end)
                 if np.isnan(result.uncertainty.value) or np.isinf(result.uncertainty.value):
                     return ''
                 return str(result.uncertainty.to_value(result.unit))
             else:
                 return ''
 
         temp_results = []
-        spec_subtracted = spectrum - continuum
 
         if spec_subtracted.mask is not None:
             # temporary fix while mask may contain None:
             spec_subtracted.mask = spec_subtracted.mask.astype(bool)
 
         for function in FUNCTIONS:
             # TODO: update specutils to allow ALL analysis to take regions and continuum so we
@@ -553,15 +420,15 @@
                                  'uncertainty': _uncertainty(temp_result),
                                  'unit': str(temp_result.unit)})
 
         if not self.selected_line and self.identified_line:
             # default to the identified line
             self.selected_line = self.identified_line
 
-        self.update_results(temp_results, mark_x, mark_y)
+        self.update_results(temp_results)
 
     def _compute_redshift_for_selected_line(self):
         index = self.line_items.index(self.selected_line)
         line_mark = self.line_marks[index]
         rest_value = (line_mark.rest_value * line_mark.xunit).to_value(u.AA,
                                                                        equivalencies=u.spectral())
         return (self.results_centroid - rest_value) / rest_value
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.vue` & `jdaviz-3.9.0/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.vue`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 <template>
   <j-tray-plugin
-    description="Return statistics for a single spectral line."
+    :description="docs_description || 'Return statistics for a single spectral line.'"
     :link="docs_link || 'https://jdaviz.readthedocs.io/en/'+vdocs+'/'+config+'/plugins.html#line-analysis'"
     :uses_active_status="uses_active_status"
     @plugin-ping="plugin_ping($event)"
     :keep_active.sync="keep_active"
     :disabled_msg="disabled_msg"
-    :popout_button="popout_button">
+    :popout_button="popout_button"
+    :scroll_to.sync="scroll_to">
 
     <j-plugin-section-header>Line</j-plugin-section-header>
     <v-row>
       <j-docs-link>Choose a region that defines the spectral line.</j-docs-link>
     </v-row>
 
     <!-- for mosviz, the entries change on row change, so we want to always show the dropdown
@@ -45,15 +46,15 @@
           Selected dataset and spectral subset do not overlap
       </span>
     </v-row>
 
     <j-plugin-section-header>Continuum</j-plugin-section-header>
     <v-row>
       <j-docs-link>
-        {{spectral_subset_selected=='Entire Spectrum' ? "Since using the entire spectrum, the end points will be used to fit a linear continuum." : "Choose a region to fit a linear line as the underlying continuum."}}  
+        {{continuum_subset_selected=='Surrounding' && spectral_subset_selected=='Entire Spectrum' ? "Since using the entire spectrum, the end points will be used to fit a linear continuum." : "Choose a region to fit a linear line as the underlying continuum."}}  
         {{continuum_subset_selected=='Surrounding' && spectral_subset_selected!='Entire Spectrum' ? "Choose a width in number of data points to consider on each side of the line region defined above." : null}}
         When this plugin is opened, a visual indicator will show on the spectrum plot showing the continuum fitted as a thick line, and interpolated into the line region as a thin line.
       </j-docs-link>
     </v-row>
 
     <plugin-subset-select 
       :items="continuum_subset_items"
@@ -66,19 +67,19 @@
 
     <v-row v-if="continuum_subset_selected=='Surrounding' && spectral_subset_selected!='Entire Spectrum'">
       <!-- DEV NOTE: if changing the validation rules below, also update the logic to clear the results
            in line_analysis.py  -->
       <v-text-field
         label="Width"
         type="number"
-        v-model.number="width"
+        v-model.number="continuum_width"
         step="0.1"
-        :rules="[() => width!=='' || 'This field is required.',
-                 () => width<=10 || 'Width must be <= 10.',
-                 () => width>=1 || 'Width must be >= 1.']"
+        :rules="[() => continuum_width!=='' || 'This field is required.',
+                 () => continuum_width<=10 || 'Width must be <= 10.',
+                 () => continuum_width>=1 || 'Width must be >= 1.']"
         hint="Width, relative to the overall line spectral region, to fit the linear continuum (excluding the region containing the line).  If 1, will use endpoints within line region only."
         persistent-hint
       >
       </v-text-field>
     </v-row>
 
     <j-plugin-section-header>Results</j-plugin-section-header>
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/specviz/plugins/line_analysis/tests/test_line_analysis.py` & `jdaviz-3.9.0/jdaviz/configs/specviz/plugins/line_analysis/tests/test_line_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-import numpy as np
-from numpy.testing import assert_allclose
 import pytest
+import numpy as np
 from astropy import units as u
 from astropy.table import QTable
+from astropy.tests.helper import assert_quantity_allclose
 from glue.core.roi import XRangeROI
 from glue.core.edit_subset_mode import NewMode
+from numpy.testing import assert_allclose
 from regions import RectanglePixelRegion, PixCoord
 from specutils import Spectrum1D
 
 from jdaviz.configs.specviz.plugins.line_analysis.line_analysis import _coerce_unit
 from jdaviz.core.events import LineIdentifyMessage
 from jdaviz.core.marks import LineAnalysisContinuum
 
@@ -171,19 +172,18 @@
     assert_allclose(z, (la_plugin.results_centroid - line_mark.rest_value)/line_mark.rest_value)
     assert_allclose(la_plugin.selected_line_redshift, z)
 
 
 def test_coerce_unit():
     q_input = 1 * u.Unit('1E-20 erg m / (Angstrom cm**2 s)')
     q_input.uncertainty = 0.1 * u.Unit('1E-20 erg m / (Angstrom cm**2 s)')
+    q_unit = u.Unit('erg / (cm**2 s)')
     q_coerced = _coerce_unit(q_input)
-    assert q_coerced.unit == u.Unit('erg / (cm**2 s)')
-    assert np.allclose(q_coerced.value, 1e-20 * u.m.to(u.Angstrom))
-    assert q_coerced.uncertainty.unit == u.Unit('erg / (cm**2 s)')
-    assert np.allclose(q_coerced.uncertainty.value, 0.1 * 1e-20 * u.m.to(u.Angstrom))
+    assert_quantity_allclose(q_coerced, 1e-10 * q_unit)
+    assert_quantity_allclose(q_coerced.uncertainty, 1e-11 * q_unit)
     q_input.uncertainty = None
     q_coerced = _coerce_unit(q_input)
     assert not hasattr(q_coerced, 'uncertainty')
 
 
 def test_continuum_surrounding_spectral_subset(specviz_helper, spectrum1d):
     label = "Test 1D Spectrum"
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/specviz/plugins/line_analysis/tests/test_lineflux.py` & `jdaviz-3.9.0/jdaviz/configs/specviz/plugins/line_analysis/tests/test_lineflux.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/specviz/plugins/parsers.py` & `jdaviz-3.9.0/jdaviz/configs/specviz/plugins/parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/specviz/plugins/unit_conversion/tests/test_unit_conversion.py` & `jdaviz-3.9.0/jdaviz/configs/specviz/plugins/unit_conversion/tests/test_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.py` & `jdaviz-3.9.0/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.vue` & `jdaviz-3.9.0/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.vue`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 <template>
   <!-- To re-enable plugin, use :disabled_msg="disabled_msg" -->
   <j-tray-plugin
-    description='Convert the spectral flux density and spectral axis units.'
+    :description="docs_description || 'Convert the spectral flux density and spectral axis units.'"
     :link="docs_link || 'https://jdaviz.readthedocs.io/en/'+vdocs+'/'+config+'/plugins.html#unit-conversion'"
     :disabled_msg="disabled_msg"
-    :popout_button="popout_button">
+    :popout_button="popout_button"
+    :scroll_to.sync="scroll_to">
 
     <v-row>
       <v-select
         :menu-props="{ left: true }"
         attach
         :items="spectral_unit_items.map(i => i.label)"
         v-model="spectral_unit_selected"
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/specviz/plugins/viewers.py` & `jdaviz-3.9.0/jdaviz/configs/specviz/plugins/viewers.py`

 * *Files 4% similar despite different names*

```diff
@@ -257,39 +257,44 @@
         fig = self.figure
         # Deselect any pan/zoom or subsetting tools so they don't interfere
         # with the scale retrieval
         if self.toolbar.active_tool is not None:
             self.toolbar.active_tool = None
         return {'x': fig.interaction.x_scale, 'y': fig.interaction.y_scale}
 
-    def plot_spectral_line(self, line, plot_units=None, **kwargs):
+    def plot_spectral_line(self, line, global_redshift=None, plot_units=None, **kwargs):
         if isinstance(line, str):
             # Try the full index first (for backend calls), otherwise name only
             try:
                 line = self.spectral_lines.loc[line]
             except KeyError:
                 line = self.spectral_lines.loc["linename", line]
         if plot_units is None:
             plot_units = self.data()[0].spectral_axis.unit
 
+        if global_redshift is None:
+            redshift = self.redshift
+        else:
+            redshift = global_redshift
+
         line_mark = SpectralLine(self,
-                                 line['rest'].to(plot_units).value,
-                                 self.redshift,
+                                 line['rest'].to_value(plot_units),
+                                 redshift,
                                  name=line["linename"],
                                  table_index=line["name_rest"],
                                  colors=[line["colors"]], **kwargs)
 
         # Erase this line if it already existed, to avoid duplication
         self.erase_spectral_lines(name_rest=line["name_rest"])
 
         self.figure.marks = self.figure.marks + [line_mark]
         line["show"] = True
         self._broadcast_plotted_lines()
 
-    def plot_spectral_lines(self, colors=["blue"], **kwargs):
+    def plot_spectral_lines(self, colors=["blue"], global_redshift=None, **kwargs):
         """
         Plots a user-provided astropy table of spectral lines in the viewer.
         """
         fig = self.figure
         self.erase_spectral_lines(show_none=False)
 
         # Check to see if colors were defined for each line
@@ -297,21 +302,26 @@
             colors = self.spectral_lines["colors"]
         elif len(colors) != len(self.spectral_lines):
             colors = colors*len(self.spectral_lines)
 
         lines = self.spectral_lines
         plot_units = self.data()[0].spectral_axis.unit
 
+        if global_redshift is None:
+            redshift = self.redshift
+        else:
+            redshift = global_redshift
+
         marks = []
         for line, color in zip(lines, colors):
             if not line["show"]:
                 continue
             line = SpectralLine(self,
-                                line['rest'].to(plot_units).value,
-                                redshift=self.redshift,
+                                line['rest'].to_value(plot_units),
+                                redshift,
                                 name=line["linename"],
                                 table_index=line["name_rest"],
                                 colors=[color], **kwargs)
             marks.append(line)
         fig.marks = fig.marks + marks
         self._broadcast_plotted_lines()
 
@@ -541,16 +551,32 @@
                                                     close_path=False
                                                     )
 
                 # Add error lines to viewer
                 self.figure.marks = list(self.figure.marks) + [error_line_mark]
 
     def set_plot_axes(self):
-        # Set axes labels for the spectrum viewer
-        flux_unit_type = "Flux density"
+        # Set y axes labels for the spectrum viewer
+        y_display_unit = self.state.y_display_unit
+        y_unit = u.Unit(y_display_unit) if y_display_unit else u.dimensionless_unscaled
+
+        if y_unit.is_equivalent(u.Jy / u.sr):
+            flux_unit_type = "Surface brightness"
+        elif y_unit.is_equivalent(u.erg / (u.s * u.cm**2)):
+            flux_unit_type = 'Flux'
+        elif y_unit.is_equivalent(u.electron / u.s) or y_unit.physical_type == 'dimensionless':
+            # electron / s or 'dimensionless_unscaled' should be labeled counts
+            flux_unit_type = "Counts"
+        elif y_unit.is_equivalent(u.W):
+            flux_unit_type = "Luminosity"
+        else:
+            # default to Flux Density for flux density or uncaught types
+            flux_unit_type = "Flux density"
+
+        # Set x axes labels for the spectrum viewer
         x_disp_unit = self.state.x_display_unit
         x_unit = u.Unit(x_disp_unit) if x_disp_unit else u.dimensionless_unscaled
         if x_unit.is_equivalent(u.m):
             spectral_axis_unit_type = "Wavelength"
         elif x_unit.is_equivalent(u.Hz):
             spectral_axis_unit_type = "Frequency"
         elif x_unit.is_equivalent(u.pixel):
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/specviz/specviz.ipynb` & `jdaviz-3.9.0/jdaviz/configs/specviz/specviz.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/specviz/tests/test_helper.py` & `jdaviz-3.9.0/jdaviz/configs/specviz/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/specviz2d/helper.py` & `jdaviz-3.9.0/jdaviz/configs/specviz2d/helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/specviz2d/plugins/parsers.py` & `jdaviz-3.9.0/jdaviz/configs/specviz2d/plugins/parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.py` & `jdaviz-3.9.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.vue` & `jdaviz-3.9.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.vue`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 <template>
   <j-tray-plugin
-    description="2D to 1D spectral extraction."
+    :description="docs_description || '2D to 1D spectral extraction.'"
     :link="docs_link || 'https://jdaviz.readthedocs.io/en/'+vdocs+'/'+config+'/plugins.html#spectral-extraction'"
     :uses_active_status="uses_active_status"
     @plugin-ping="plugin_ping($event)"
     :keep_active.sync="keep_active"
-    :popout_button="popout_button">
+    :popout_button="popout_button"
+    :scroll_to.sync="scroll_to">
 
     <v-row>
       <v-expansion-panels popout>
         <v-expansion-panel>
           <v-expansion-panel-header v-slot="{ open }">
             <span style="padding: 6px">Settings</span>
           </v-expansion-panel-header>
@@ -25,15 +26,15 @@
           </v-expansion-panel-content>
         </v-expansion-panel>
       </v-expansion-panels>
     </v-row>
 
 
     <div @mouseover="() => active_step='trace'">
-      <j-plugin-section-header>Trace</j-plugin-section-header>
+      <j-plugin-section-header :active="active_step==='trace'">Trace</j-plugin-section-header>
       <v-row>
         <j-docs-link>
           Create a trace for the spectrum.  See the <j-external-link link='https://specreduce.readthedocs.io/en/latest/#module-specreduce.tracing' linktext='specreduce docs'></j-external-link> for more details on the available trace types.
         </j-docs-link>
       </v-row>
 
       <plugin-dataset-select
@@ -185,15 +186,15 @@
             </v-expansion-panel-content>
           </v-expansion-panel>
         </v-expansion-panels>
       </v-row>
     </div>
 
     <div @mouseover="() => active_step='bg'">
-      <j-plugin-section-header>Background</j-plugin-section-header>
+      <j-plugin-section-header :active="active_step==='bg'">Background</j-plugin-section-header>
       <v-row>
         <j-docs-link>Create a background and/or background-subtracted image.</j-docs-link>
       </v-row>
 
       <v-row v-if="ext_dataset_selected !== 'From Plugin'">
         <span class="v-messages v-messages__message text--secondary">
           <b style="color: red !important">NOTE:</b> extracted spectrum is using "{{ext_dataset_selected}}" as input data, so will not update in real-time.  Switch to "From Plugin" to use the background subtraction defined here.
@@ -348,15 +349,15 @@
             </v-expansion-panel-content>
           </v-expansion-panel>
         </v-expansion-panels>
       </v-row>
     </div>
 
     <div @mouseover="() => active_step='ext'">
-      <j-plugin-section-header>Extraction</j-plugin-section-header>
+      <j-plugin-section-header :active="active_step==='ext'">Extraction</j-plugin-section-header>
       <v-row>
         <j-docs-link>
           Extract a 1D spectrum from a 2D spectrum.  See the <j-external-link link='https://specreduce.readthedocs.io/en/latest/#module-specreduce.extract' linktext='specreduce docs'></j-external-link> for more details on the available extraction methods.
         </j-docs-link>
       </v-row>
 
       <plugin-dataset-select
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/test_spectral_extraction.py` & `jdaviz-3.9.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/test_spectral_extraction.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
     pext = specviz2d_helper.plugins['Spectral Extraction']
     pext.keep_active = True
 
     # test that setting a string to an AddResults object redirects to the label
     pext.bg_sub_add_results = 'override label'
     assert pext.bg_sub_add_results.label == 'override label'
     pext.bg_sub_add_results.label = 'override label 2'
-    assert "override label 2" in pext.bg_sub_add_results.__repr__()
+    assert "override label 2" in pext.bg_sub_add_results._obj.__repr__()
     assert "override label 2" in pext.bg_sub_add_results._obj.auto_label.__repr__()
 
     pext.export_bg_sub(add_data=True)
     assert 'override label 2' in pext.ext_dataset.choices
 
     # test setting auto label
     pext.bg_sub_add_results.auto = True
```

### Comparing `jdaviz-3.8.2/jdaviz/configs/specviz2d/tests/test_helper.py` & `jdaviz-3.9.0/jdaviz/configs/specviz2d/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/configs/specviz2d/tests/test_parsers.py` & `jdaviz-3.9.0/jdaviz/configs/specviz2d/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/conftest.py` & `jdaviz-3.9.0/jdaviz/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # This file is used to configure the behavior of pytest when using the Astropy
 # test infrastructure. It needs to live inside the package in order for it to
 # get picked up when running the tests inside an interpreter using
 # packagename.test
 
+import os
 import warnings
 
 import numpy as np
 import pytest
 from astropy import units as u
 from astropy.io import fits
 from astropy.nddata import CCDData, StdDevUncertainty
@@ -95,15 +96,19 @@
     uncert_hdu.header['BUNIT'] = '1E-17 erg*s^-1*cm^-2*Angstrom^-1'
 
     return fits.HDUList([fits.PrimaryHDU(), flux_hdu, uncert_hdu, mask_hdu])
 
 
 @pytest.fixture
 def image_cube_hdu_obj_microns():
-    flux_hdu = fits.ImageHDU(np.ones((8, 9, 10)).astype(np.float32))
+    # Basic rectangle ramp for aperture photometry test.
+    a = np.zeros((8, 9, 10)).astype(np.float32)  # (nz, ny, nx)
+    for i in range(8):
+        a[i, :5, :3] = i + 1
+    flux_hdu = fits.ImageHDU(a)
     flux_hdu.name = 'FLUX'
 
     uncert_hdu = fits.ImageHDU(np.zeros((8, 9, 10)).astype(np.float32))
     uncert_hdu.name = 'ERR'
 
     mask_hdu = fits.ImageHDU(np.ones((8, 9, 10)).astype(np.uint16))
     mask_hdu.name = 'MASK'
@@ -200,24 +205,27 @@
 
 def _create_spectrum1d_cube_with_fluxunit(fluxunit=u.Jy, shape=(2, 2, 4), with_uncerts=False):
     # nz=2 nx=2 ny=4
     flux = np.arange(np.prod(shape)).reshape(shape) * fluxunit
     wcs_dict = {"CTYPE1": "RA---TAN", "CTYPE2": "DEC--TAN", "CTYPE3": "WAVE-LOG",
                 "CRVAL1": 205, "CRVAL2": 27, "CRVAL3": 4.622e-7,
                 "CDELT1": -0.0001, "CDELT2": 0.0001, "CDELT3": 8e-11,
-                "CRPIX1": 0, "CRPIX2": 0, "CRPIX3": 0}
+                "CRPIX1": 0, "CRPIX2": 0, "CRPIX3": 0,
+                # Need these for aperture photometry test.
+                "TELESCOP": "JWST", "BUNIT": fluxunit.to_string(), "PIXAR_A2": 0.01}
     w = WCS(wcs_dict)
     if with_uncerts:
         uncert = StdDevUncertainty(np.abs(np.random.normal(flux) * u.Jy))
 
         return Spectrum1D(flux=flux,
                           uncertainty=uncert,
-                          wcs=w)
+                          wcs=w,
+                          meta=wcs_dict)
     else:
-        return Spectrum1D(flux=flux, wcs=w)
+        return Spectrum1D(flux=flux, wcs=w, meta=wcs_dict)
 
 
 @pytest.fixture
 def spectrum1d_cube():
     return _create_spectrum1d_cube_with_fluxunit(fluxunit=u.Jy)
 
 
@@ -228,14 +236,26 @@
 
 @pytest.fixture
 def spectrum1d_cube_larger():
     return _create_spectrum1d_cube_with_fluxunit(fluxunit=u.Jy, shape=(SPECTRUM_SIZE, 2, 4))
 
 
 @pytest.fixture
+def spectrum1d_cube_largest():
+    wcs_dict = {"CTYPE1": "WAVE-LOG", "CTYPE2": "DEC--TAN", "CTYPE3": "RA---TAN",
+                "CRVAL1": 4.622e-7, "CRVAL2": 27, "CRVAL3": 205,
+                "CDELT1": 8e-11, "CDELT2": 0.0001, "CDELT3": -0.0001,
+                "CRPIX1": 0, "CRPIX2": 0, "CRPIX3": 0}
+    w = WCS(wcs_dict)
+    flux = np.zeros((30, 20, 3001), dtype=np.float32)  # nx=20 ny=30 nz=3001
+    flux[5:15, 1:11, :] = 1  # Bright corner
+    return Spectrum1D(flux=flux * u.Jy, wcs=w, meta=wcs_dict)
+
+
+@pytest.fixture
 def spectrum1d_cube_custom_fluxunit():
     return _create_spectrum1d_cube_with_fluxunit
 
 
 @pytest.fixture
 def mos_spectrum1d(mos_spectrum2d):
     '''
@@ -311,14 +331,26 @@
 
 @pytest.fixture
 def roman_imagemodel():
     if HAS_ROMAN_DATAMODELS:
         return create_wfi_image_model((20, 10))
 
 
+# Copied over from https://github.com/spacetelescope/ci_watson
+@pytest.fixture(scope='function')
+def _jail(tmp_path):
+    """Perform test in a pristine temporary working directory."""
+    old_dir = os.getcwd()
+    os.chdir(tmp_path)
+    try:
+        yield str(tmp_path)
+    finally:
+        os.chdir(old_dir)
+
+
 try:
     from pytest_astropy_header.display import PYTEST_HEADER_MODULES, TESTED_VERSIONS
 except ImportError:
     PYTEST_HEADER_MODULES = {}
     TESTED_VERSIONS = {}
```

### Comparing `jdaviz-3.8.2/jdaviz/container.vue` & `jdaviz-3.9.0/jdaviz/container.vue`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
       :layer_icons="layer_icons"
       @resize="(e) => $emit('resize', e)"
       :closefn="closefn"
       @data-item-visibility="$emit('data-item-visibility', $event)"
       @data-item-unload="$emit('data-item-unload', $event)"
       @data-item-remove="$emit('data-item-remove', $event)"
       @call-viewer-method="$emit('call-viewer-method', $event)"
+      @change-reference-data="$emit('change-reference-data', $event)"
     ></g-viewer-tab>
     <gl-component
       v-for="(viewer, index) in stack.viewers"
       :key="viewer.id"
       :title="viewer.reference || viewer.id"
       :tab-id="viewer.id"
       @resize="(e) => $emit('resize', e)"
@@ -29,20 +30,21 @@
           <v-row dense style="background-color: #205f76; margin: 0px" class="jdaviz-viewer-toolbar">
             <j-viewer-data-select
               :data_items="data_items" 
               :viewer="viewer"
               :app_settings="app_settings"
               :layer_icons="layer_icons"
               :icons="icons"
+              :linked_by_wcs="viewer.linked_by_wcs"
               @data-item-visibility="$emit('data-item-visibility', $event)"
               @data-item-unload="$emit('data-item-unload', $event)"
               @data-item-remove="$emit('data-item-remove', $event)"
+              @change-reference-data="$emit('change-reference-data', $event)"
             ></j-viewer-data-select>
 
-
             <v-toolbar-items v-if="viewer.reference === 'table-viewer'">
               <j-tooltip tipid='table-prev'>
                 <v-btn icon @click="$emit('call-viewer-method', {'id': viewer.id, 'method': 'prev_row'})" color="white">
                   <v-icon>mdi-arrow-up-bold</v-icon>
                 </v-btn>
               </j-tooltip>
               <j-tooltip tipid='table-next'>
@@ -58,22 +60,22 @@
 
         </div>
 
         <v-card tile flat style="flex: 1; margin-top: -2px; overflow: hidden;">
           <div v-if="app_settings.viewer_labels" class='viewer-label-container'>
             <div v-if="Object.keys(viewer_icons).length > 1" class="viewer-label invert-if-dark">
               <j-tooltip span_style="white-space: nowrap">
-                <j-layer-viewer-icon span_style="float: right;" :icon="viewer_icons[viewer.id]"></j-layer-viewer-icon>
+                <j-layer-viewer-icon span_style="float: right;" :icon="viewer_icons[viewer.id]" :linked_by_wcs="viewer.linked_by_wcs"></j-layer-viewer-icon>
               </j-tooltip>
               <span class="invert-if-dark" style="margin-left: 24px; margin-right: 32px; line-height: 24px">{{viewer.reference || viewer.id}}</span>
             </div>
 
             <div v-for="(layer_info, layer_name) in viewer.visible_layers" class="viewer-label invert-if-dark">
               <j-tooltip span_style="white-space: nowrap">
-                <j-layer-viewer-icon span_style="float: right;" :icon="layer_icons[layer_name]" :linewidth="layer_info.linewidth" :linestyle="'solid'" :color="layer_info.color"></j-layer-viewer-icon>
+                <j-layer-viewer-icon span_style="float: right;" :icon="layer_icons[layer_name]" :linewidth="layer_info.linewidth" :linestyle="'solid'" :color="layer_info.color" :linked_by_wcs="viewer.linked_by_wcs"></j-layer-viewer-icon>
               </j-tooltip>
               <span class="invert-if-dark" style="margin-left: 24px; margin-right: 32px; line-height: 24px">
                 <v-icon v-if="layer_info.prefix_icon" dense>
                   {{layer_info.prefix_icon}}
                 </v-icon>
                 {{layer_name}}{{layer_info.suffix_label}}
               </span>
```

### Comparing `jdaviz-3.8.2/jdaviz/core/astrowidgets_api.py` & `jdaviz-3.9.0/jdaviz/core/astrowidgets_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from astropy import units as u
 from astropy.coordinates import SkyCoord
 from astropy.wcs import NoConvergence
 from echo import delay_callback
 from glue.config import colormaps
 from glue.core import Data
 
-from jdaviz.configs.imviz.helper import get_top_layer_index
-from jdaviz.core.events import SnackbarMessage, MarkersChangedMessage
+from jdaviz.configs.imviz.helper import get_top_layer_index, get_reference_image_data
+from jdaviz.core.events import SnackbarMessage, AstrowidgetMarkersChangedMessage
 from jdaviz.core.helpers import data_has_valid_wcs
 
 __all__ = ['AstrowidgetsImageViewerMixin']
 
 
 class AstrowidgetsImageViewerMixin:
     """This class implements ``astrowidgets`` API for Jdaviz *image* viewer.
@@ -73,14 +73,17 @@
         Raises
         ------
         AttributeError
             Sky coordinates are given but image does not have a valid WCS.
 
         """
         i_top = get_top_layer_index(self)
+        if i_top is None:
+            return
+
         image = self.layers[i_top].layer
 
         if isinstance(point, SkyCoord):
             if data_has_valid_wcs(image):
                 try:
                     point = image.coords.world_to_pixel(point)  # 0-indexed X, Y
                 except NoConvergence as e:  # pragma: no cover
@@ -127,98 +130,128 @@
         ValueError
             Offsets are of different types.
 
         astropy.units.core.UnitTypeError
             Sky offset has invalid unit.
 
         """
+        i_top = get_top_layer_index(self)
+        image = self.layers[i_top].layer
         width = self.state.x_max - self.state.x_min
         height = self.state.y_max - self.state.y_min
+        x_cen = self.state.x_min + (width * 0.5)
+        y_cen = self.state.y_min + (height * 0.5)
+        if hasattr(self, '_get_real_xy'):
+            real_cen = self._get_real_xy(image, x_cen, y_cen)
+        else:
+            real_cen = (x_cen, y_cen)
 
         dx, dx_coord = _offset_is_pixel_or_sky(dx)
         dy, dy_coord = _offset_is_pixel_or_sky(dy)
 
         if dx_coord != dy_coord:
             raise ValueError(f'dx is of type {dx_coord} but dy is of type {dy_coord}')
 
         if dx_coord == 'wcs':
-            i_top = get_top_layer_index(self)
-            image = self.layers[i_top].layer
             if data_has_valid_wcs(image):
                 # To avoid distortion headache, assume offset is relative to
                 # displayed center.
-                x_cen = self.state.x_min + (width * 0.5)
-                y_cen = self.state.y_min + (height * 0.5)
-                sky_cen = image.coords.pixel_to_world(x_cen, y_cen)
-                new_sky_cen = sky_cen.spherical_offsets_by(dx, dy)
-                self.center_on(new_sky_cen)
+                sky_cen = image.coords.pixel_to_world(real_cen[0], real_cen[1])
+                new_cen = sky_cen.spherical_offsets_by(dx, dy)
             else:
                 raise AttributeError(f'{getattr(image, "label", None)} does not have a valid WCS')
         else:
-            with delay_callback(self.state, 'x_min', 'x_max', 'y_min', 'y_max'):
-                self.state.x_min += dx
-                self.state.y_min += dy
-                self.state.x_max = self.state.x_min + width
-                self.state.y_max = self.state.y_min + height
+            new_cen = (real_cen[0] + dx, real_cen[1] + dy)
+
+        self.center_on(new_cen)
 
     @property
     def zoom_level(self):
-        """Zoom level:
+        """
+        The zoom level for an image viewer (not linked by WCS).
+
+        .. warning::
+            When a viewer is linked by WCS, the result corresponds
+            to the ``zoom_level`` of the reference data.
 
         * 1 means real-pixel-size.
         * 2 means zoomed in by a factor of 2.
         * 0.5 means zoomed out by a factor of 2.
         * 'fit' means zoomed to fit the whole image width into display.
 
         """
         if self.shape is None:  # pragma: no cover
             raise ValueError('Viewer is still loading, try again later')
 
+        if hasattr(self, '_get_real_xy'):
+            image, i_ref = get_reference_image_data(self.jdaviz_app, self.reference)
+            # TODO: Do we want top layer instead?
+            # i_top = get_top_layer_index(self)
+            # image = self.layers[i_top].layer
+            real_min = self._get_real_xy(image, self.state.x_min, self.state.y_min)
+            real_max = self._get_real_xy(image, self.state.x_max, self.state.y_max)
+        else:
+            real_min = (self.state.x_min, self.state.y_min)
+            real_max = (self.state.x_max, self.state.y_max)
         screenx = self.shape[1]
         screeny = self.shape[0]
-        zoom_x = screenx / (self.state.x_max - self.state.x_min)
-        zoom_y = screeny / (self.state.y_max - self.state.y_min)
+        zoom_x = screenx / abs(real_max[0] - real_min[0])
+        zoom_y = screeny / abs(real_max[1] - real_min[1])
 
         return max(zoom_x, zoom_y)  # Similar to Ginga get_scale()
 
     # Loosely based on glue/viewers/image/state.py
     @zoom_level.setter
     def zoom_level(self, val):
         if ((not isinstance(val, (int, float)) and val != 'fit') or
                 (isinstance(val, (int, float)) and val <= 0)):
             raise ValueError(f'Unsupported zoom level: {val}')
 
-        image = self.state.reference_data
-        if (image is None or self.shape is None or
+        if (self.shape is None or
                 self.state.x_att is None or self.state.y_att is None):  # pragma: no cover
             return
 
         # Zoom on X and Y will auto-adjust.
         if val == 'fit':
             self.state.reset_limits()
             return
+
+        new_dx = self.shape[1] * 0.5 / val
+        if hasattr(self, '_get_real_xy'):
+            image, i_ref = get_reference_image_data(self.jdaviz_app, self.reference)
+            # TODO: Do we want top layer instead?
+            # i_top = get_top_layer_index(self)
+            # image = self.layers[i_top].layer
+            real_min = self._get_real_xy(image, self.state.x_min, self.state.y_min)
+            real_max = self._get_real_xy(image, self.state.x_max, self.state.y_max)
+            cur_xcen = (real_min[0] + real_max[0]) * 0.5
+            new_x_min = self._get_real_xy(image, cur_xcen - new_dx - 0.5, real_min[1], reverse=True)[0]  # noqa: E501
+            new_x_max = self._get_real_xy(image, cur_xcen + new_dx - 0.5, real_max[1], reverse=True)[0]  # noqa: E501
         else:
             cur_xcen = (self.state.x_min + self.state.x_max) * 0.5
-            new_dx = self.shape[1] * 0.5 / val
-            new_x_min = cur_xcen - new_dx
-            new_x_max = cur_xcen + new_dx
+            new_x_min = cur_xcen - new_dx - 0.5
+            new_x_max = cur_xcen + new_dx - 0.5
 
         with delay_callback(self.state, 'x_min', 'x_max'):
-            self.state.x_min = new_x_min - 0.5
-            self.state.x_max = new_x_max - 0.5
+            self.state.x_min = new_x_min
+            self.state.x_max = new_x_max
 
         # We need to adjust the limits in here to avoid triggering all
         # the update events then changing the limits again.
         self.state._adjust_limits_aspect()
 
     # Discussion on why we need two different ways to set zoom at
     # https://github.com/astropy/astrowidgets/issues/144
     def zoom(self, val):
         """Zoom in or out by the given factor.
 
+        .. warning::
+            When a viewer is linked by WCS, this method accidentally
+            changes the center also; see the warning in ``zoom_level``.
+
         Parameters
         ----------
         val : int or float
             The zoom level to zoom the image.
             See `zoom_level`.
 
         Raises
@@ -447,16 +480,20 @@
 
         if marker_name is None:
             marker_name = self._default_mark_tag_name
 
         self._validate_marker_name(marker_name)
         jglue = self.session.application
 
-        # Link markers to reference image data.
-        image = self.state.reference_data
+        # Link markers to top visible image data or reference data.
+        if not use_skycoord and hasattr(self, '_get_real_xy'):
+            i_top = get_top_layer_index(self)
+            image = self.layers[i_top].layer
+        else:
+            image = self.state.reference_data
 
         # TODO: Is Glue smart enough to no-op if link already there?
         if use_skycoord:
             if not data_has_valid_wcs(image):
                 raise AttributeError(f'{getattr(image, "label", None)} does not have a valid WCS')
             sky = table[skycoord_colname]
             t_glue = Data(marker_name, ra=sky.ra.deg, dec=sky.dec.deg)
@@ -496,15 +533,15 @@
                     break
 
             self.jdaviz_app.set_data_visibility(self.reference_id, marker_name,
                                                 visible=True, replace=False)
 
             self._marktags.add(marker_name)
 
-            self.session.hub.broadcast(MarkersChangedMessage(True, sender=self))
+            self.session.hub.broadcast(AstrowidgetMarkersChangedMessage(True, sender=self))
 
     def remove_markers(self, marker_name=None):
         """Remove some but not all of the markers by name used when
         adding the markers.
 
         Parameters
         ----------
@@ -531,15 +568,16 @@
                 color="warning", sender=self))
             return
 
         data = self.session.application.data_collection[i]
         self.session.application.data_collection.remove(data)
         self._marktags.remove(marker_name)
 
-        self.session.hub.broadcast(MarkersChangedMessage(len(self._marktags) > 0, sender=self))
+        self.session.hub.broadcast(AstrowidgetMarkersChangedMessage(len(self._marktags) > 0,
+                                                                    sender=self))
 
     def reset_markers(self):
         """Delete all markers."""
         # Grab the entire list of marker names before iterating
         # otherwise what we are iterating over changes.
         for marker_name in list(self._marktags):
             self.remove_markers(marker_name=marker_name)
```

### Comparing `jdaviz-3.8.2/jdaviz/core/config.py` & `jdaviz-3.9.0/jdaviz/core/config.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/core/custom_traitlets.py` & `jdaviz-3.9.0/jdaviz/core/custom_traitlets.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/core/data_formats.py` & `jdaviz-3.9.0/jdaviz/core/data_formats.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/core/events.py` & `jdaviz-3.9.0/jdaviz/core/events.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import astropy.units as u
 from glue.core.message import Message
 
 __all__ = ['NewViewerMessage', 'ViewerAddedMessage', 'ViewerRemovedMessage', 'LoadDataMessage',
            'AddDataMessage', 'SnackbarMessage', 'RemoveDataMessage',
            'AddLineListMessage', 'RowLockMessage',
-           'SliceSelectSliceMessage',
+           'SliceSelectSliceMessage', 'SliceValueUpdatedMessage',
            'SliceToolStateMessage',
            'TableClickMessage', 'LinkUpdatedMessage', 'ExitBatchLoadMessage',
-           'MarkersChangedMessage', 'CanvasRotationChangedMessage',
-           'GlobalDisplayUnitChanged']
+           'AstrowidgetMarkersChangedMessage', 'MarkersPluginUpdate',
+           'CanvasRotationChangedMessage',
+           'GlobalDisplayUnitChanged', 'ChangeRefDataMessage',
+           'PluginTableAddedMessage', 'PluginTableModifiedMessage',
+           'PluginPlotAddedMessage', 'PluginPlotModifiedMessage']
 
 
 class NewViewerMessage(Message):
     """Message to trigger viewer creation in the application."""
     def __init__(self, cls, data, x_attr=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
@@ -125,14 +128,40 @@
         return self._viewer
 
     @property
     def viewer_id(self):
         return self._viewer_id
 
 
+class ChangeRefDataMessage(Message):
+    def __init__(self, data, viewer, viewer_id=None, old=None, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        self._data = data
+        self._viewer = viewer
+        self._viewer_id = viewer_id
+        self._old = old
+
+    @property
+    def data(self):
+        return self._data
+
+    @property
+    def viewer(self):
+        return self._viewer
+
+    @property
+    def viewer_id(self):
+        return self._viewer_id
+
+    @property
+    def old(self):
+        return self._old
+
+
 class SnackbarMessage(Message):
     def __init__(self, text, color=None, timeout=5000, loading=False,
                  *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self._text = text
         self._color = color
@@ -275,33 +304,46 @@
     def shared_image(self):
         return self._shared_image
 
 
 class SliceSelectSliceMessage(Message):
     '''Message generated by the cubeviz helper and processed by the slice plugin to sync
     slice selection across all viewers'''
-    def __init__(self, slice=None, *args, **kwargs):
+    def __init__(self, value, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self._slice = slice
+        self._value = value
 
     @property
-    def slice(self):
-        return self._slice
+    def value(self):
+        return self._value
+
+
+class SliceValueUpdatedMessage(Message):
+    '''Message generated by the slice plugin when the selected slice is updated'''
+    def __init__(self, value, value_unit, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.value = value
+        self.value_unit = value_unit
 
 
 class SliceToolStateMessage(Message):
     '''Message generated by the select slice plot plugin when activated/deactivated'''
-    def __init__(self, change, *args, **kwargs):
+    def __init__(self, change, viewer, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._change = change
+        self._viewer = viewer
 
     @property
     def change(self):
         return self._change
 
+    @property
+    def viewer(self):
+        return self._viewer
+
 
 class LinkUpdatedMessage(Message):
     '''Message generated when the WCS/pixel linking is changed'''
     def __init__(self, link_type, wcs_use_fallback, wcs_use_affine, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._link_type = link_type
         self._wcs_use_fallback = wcs_use_fallback
@@ -322,25 +364,32 @@
 
 class ExitBatchLoadMessage(Message):
     '''Message generated when exiting the outermost batch_load context manager'''
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
-class MarkersChangedMessage(Message):
-    '''Message generated when markers are added/removed from an image viewer'''
+class AstrowidgetMarkersChangedMessage(Message):
+    '''Message generated when markers are added/removed from an image viewer via astrowidgets API'''
     def __init__(self, has_markers, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._has_markers = has_markers
 
     @property
     def has_markers(self):
         return self._has_markers
 
 
+class MarkersPluginUpdate(Message):
+    '''Message when the length of the markers plugin table changes'''
+    def __init__(self, table_length, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.table_length = table_length
+
+
 class CanvasRotationChangedMessage(Message):
     '''Message generated by canvas rotation plugin'''
     def __init__(self, viewer_id, angle, flip_horizontal, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._viewer_id = viewer_id
         self._angle = angle
         self._flip_horizontal = flip_horizontal
@@ -368,7 +417,47 @@
     @property
     def axis(self):
         return self._axis
 
     @property
     def unit(self):
         return u.Unit(self._unit)
+
+
+class PluginTableAddedMessage(Message):
+    '''Message generated when a plugin table is initialized'''
+    def __init__(self, sender):
+        super().__init__(sender)
+
+    @property
+    def table(self):
+        return self.sender
+
+    @property
+    def plugin(self):
+        return self.sender._plugin
+
+
+class PluginTableModifiedMessage(PluginTableAddedMessage):
+    '''Message generated when the items in a plugin table are changed'''
+    def __init__(self, sender):
+        super().__init__(sender)
+
+
+class PluginPlotAddedMessage(Message):
+    '''Message generated when a plugin plot is initialized'''
+    def __init__(self, sender):
+        super().__init__(sender)
+
+    @property
+    def plot(self):
+        return self.sender
+
+    @property
+    def plugin(self):
+        return self.sender._plugin
+
+
+class PluginPlotModifiedMessage(PluginPlotAddedMessage):
+    '''Message generated when the items in a plugin plot are changed'''
+    def __init__(self, sender):
+        super().__init__(sender)
```

### Comparing `jdaviz-3.8.2/jdaviz/core/helpers.py` & `jdaviz-3.9.0/jdaviz/core/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,29 +9,29 @@
 import re
 import warnings
 from contextlib import contextmanager
 from inspect import isclass
 
 import numpy as np
 import astropy.units as u
-from astropy.wcs.wcsapi import BaseHighLevelWCS
 from astropy.nddata import CCDData, StdDevUncertainty
 from regions.core.core import Region
 from glue.core import HubListener
 from glue.core.edit_subset_mode import NewMode
 from glue.core.message import SubsetCreateMessage, SubsetDeleteMessage
 from glue.core.subset import Subset, MaskSubsetState
 from glue.config import data_translator
 from ipywidgets.widgets import widget_serialization
 from specutils import Spectrum1D, SpectralRegion
 
 
 from jdaviz.app import Application
 from jdaviz.core.events import SnackbarMessage, ExitBatchLoadMessage
 from jdaviz.core.template_mixin import show_widget
+from jdaviz.utils import data_has_valid_wcs
 
 __all__ = ['ConfigHelper', 'ImageConfigHelper']
 
 
 class ConfigHelper(HubListener):
     """The Base Helper Class.
     Provides shared abstracted helper methods to the user.
@@ -106,25 +106,57 @@
 
     def load_data(self, data, data_label=None, parser_reference=None, **kwargs):
         if data_label:
             kwargs['data_label'] = data_label
         self.app.load_data(data, parser_reference=parser_reference, **kwargs)
 
     @property
+    def data_labels(self):
+        """
+        List of data labels loaded and available in jdaviz
+
+        Returns
+        -------
+        data_labels : list
+            list of strings
+        """
+        return [data.label for data in self.app.data_collection]
+
+    @property
     def plugins(self):
         """
         Access API objects for plugins in the plugin tray.
 
         Returns
         -------
         plugins : dict
             dict of plugin objects
         """
-        return {item['label']: widget_serialization['from_json'](item['widget'], None).user_api
-                for item in self.app.state.tray_items}
+        plugins = {item['label']: widget_serialization['from_json'](item['widget'], None).user_api
+                   for item in self.app.state.tray_items if item['is_relevant']}
+
+        # handle renamed plugins during deprecation
+        if 'Orientation' in plugins:
+            plugins['Links Control'] = plugins['Orientation']._obj.user_api
+            plugins['Links Control']._deprecation_msg = 'in the future, the formerly named \"Links Control\" plugin will only be available by its new name: \"Orientation\".'  # noqa
+        if 'Canvas Rotation' in plugins:
+            plugins['Canvas Rotation']._deprecation_msg = 'this functionality will be removed in favor of the implementation for rotation in the \"Orientation\" plugin.'  # noqa
+        if 'Export' in plugins:
+            plugins['Export Plot'] = plugins['Export']._obj.user_api
+            plugins['Export Plot']._deprecation_msg = 'in the future, the formerly named \"Export Plot\" plugin will only be available by its new name: \"Export\".'  # noqa
+
+        return plugins
+
+    @property
+    def plugin_tables(self):
+        return self.app._plugin_tables
+
+    @property
+    def plugin_plots(self):
+        return self.app._plugin_plots
 
     @property
     def viewers(self):
         """
         Access API objects for any viewer.
 
         Returns
@@ -681,35 +713,33 @@
         ----------
         regions : list of obj
             A list of region objects. A region object can be one of the following:
 
             * Astropy ``regions`` object
             * ``photutils`` apertures (limited support until ``photutils``
               fully supports ``regions``)
-            * Numpy boolean array (shape must match data, dtype should be ``np.bool_``)
 
         max_num_regions : int or `None`
             Maximum number of regions to load, starting from top of the list.
             Default is to load everything.
 
         refdata_label : str or `None`
             Label of data to use for sky-to-pixel conversion for a region, or
             mask creation. Data must already be loaded into Jdaviz.
             If `None`, defaults to the reference data in the default viewer.
-            Choice of this data is particularly important when sky or masked
+            Choice of this data is particularly important when sky
             region is involved.
 
         return_bad_regions : bool
             If `True`, return the regions that failed to load (see ``bad_regions``);
             This is useful for debugging. If `False`, do not return anything (`None`).
 
         kwargs : dict
             Extra keywords to be passed into the region's ``to_mask`` method.
-            **This is ignored if the region can be made interactive or
-            if a Numpy array is given.**
+            **This is ignored if the region can be made interactive.**
 
         Returns
         -------
         bad_regions : list of (obj, str) or `None`
             If requested (see ``return_bad_regions`` option), return a
             list of ``(region, reason)`` tuples for region objects that failed to load.
             If all the regions loaded successfully, this list will be empty.
@@ -755,14 +785,22 @@
                                     SkyRectangularAperture, SkyCircularAnnulus,
                                     CircleSkyRegion, EllipseSkyRegion,
                                     RectangleSkyRegion, CircleAnnulusSkyRegion))
                     and not has_wcs):
                 bad_regions.append((region, 'Sky region provided but data has no valid WCS'))
                 continue
 
+            if (isinstance(region, (CircularAperture, EllipticalAperture,
+                                    RectangularAperture, CircularAnnulus,
+                                    CirclePixelRegion, EllipsePixelRegion,
+                                    RectanglePixelRegion, CircleAnnulusPixelRegion))
+                    and self.app._link_type == "wcs"):
+                bad_regions.append((region, 'Pixel region provided by data is linked by WCS'))
+                continue
+
             # photutils: Convert to regions shape first
             if isinstance(region, (CircularAperture, SkyCircularAperture,
                                    EllipticalAperture, SkyEllipticalAperture,
                                    RectangularAperture, SkyRectangularAperture,
                                    CircularAnnulus, SkyCircularAnnulus)):
                 region = aperture2regions(region)
 
@@ -792,14 +830,15 @@
                     try:
                         mask = region.to_mask(**kwargs)
                         im = mask.to_image(data.shape)  # Can be None
                     except Exception as e:  # pragma: no cover
                         bad_regions.append((region, f'Failed to load: {repr(e)}'))
                         continue
 
+                # Boolean mask as input is supported but not advertised.
                 elif (isinstance(region, np.ndarray) and region.shape == data.shape
                         and region.dtype == np.bool_):
                     im = region
 
                 if im is None:
                     bad_regions.append((region, 'Mask creation failed'))
                     continue
@@ -847,16 +886,19 @@
         Returns
         -------
         regions : dict
             Dictionary mapping interactive region names to respective Astropy
             ``regions`` objects.
 
         """
+        from glue_astronomy.translators.regions import roi_subset_state_to_region
+
         regions = {}
         failed_regs = set()
+        to_sky = self.app._link_type == 'wcs'
 
         # Subset is global, so we just use default viewer.
         for lyr in self.default_viewer._obj.layers:
             if (not hasattr(lyr, 'layer') or not isinstance(lyr.layer, Subset)
                     or lyr.layer.ndim not in (2, 3)):
                 continue
 
@@ -865,16 +907,19 @@
 
             # TODO: Remove this when Jdaviz support round-tripping, see
             # https://github.com/spacetelescope/jdaviz/pull/721
             if not subset_label.startswith('Subset'):
                 continue
 
             try:
-                region = subset_data.data.get_selection_definition(
-                    subset_id=subset_label, format='astropy-regions')
+                if self.app.config == "imviz" and to_sky:
+                    region = roi_subset_state_to_region(subset_data.subset_state, to_sky=to_sky)
+                else:
+                    region = subset_data.data.get_selection_definition(
+                        subset_id=subset_label, format='astropy-regions')
             except (NotImplementedError, ValueError):
                 failed_regs.add(subset_label)
             else:
                 regions[subset_label] = region
 
         if len(failed_regs) > 0:
             self.app.hub.broadcast(SnackbarMessage(
@@ -909,22 +954,14 @@
     # TODO: Make this public API?
     def _delete_all_regions(self):
         """Delete all regions."""
         for subset_grp in self.app.data_collection.subset_groups:  # should be a copy
             self.app.data_collection.remove_subset_group(subset_grp)
 
 
-def data_has_valid_wcs(data, ndim=None):
-    """Check if given glue Data has WCS that is compatible with APE 14."""
-    status = hasattr(data, 'coords') and isinstance(data.coords, BaseHighLevelWCS)
-    if ndim is not None:
-        status = status and data.coords.world_n_dim == ndim
-    return status
-
-
 def _next_subset_num(label_prefix, subset_groups):
     """Assumes ``prefix i`` format.
     Does not go back and fill in lower but available numbers. This is consistent with Glue.
     """
     max_i = 0
 
     for sg in subset_groups:
```

### Comparing `jdaviz-3.8.2/jdaviz/core/launcher.py` & `jdaviz-3.9.0/jdaviz/core/launcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
         The path to the file to load into Jdaviz. Will autopopulate the File Path field
 
     height: int, optional
         The height of the top-level application widget, in pixels. Will be passed and processed
         by the selected configuration. Applies to the launcher and all instances of the same
         application in the notebook.
     '''
-    # Color defined manually due to the custom theme not being defined yet (in app.vue)
+    # Color defined manually due to the custom theme not being defined yet (in main_styles.vue)
     height = f"{height}px" if isinstance(height, int) else height
     main = v.Sheet(class_="mx-25",
                    attributes={"id": "popout-widget-container"},
                    color="#00212C",
                    height=height,
                    _metadata={'mount_id': 'content'})
     main.children = [Launcher(main, configs, filepath, height)]
```

### Comparing `jdaviz-3.8.2/jdaviz/core/launcher.vue` & `jdaviz-3.9.0/jdaviz/core/launcher.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/core/linelists.py` & `jdaviz-3.9.0/jdaviz/core/linelists.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/core/marks.py` & `jdaviz-3.9.0/jdaviz/core/marks.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,16 @@
                                 RedshiftMessage)
 
 __all__ = ['OffscreenLinesMarks', 'BaseSpectrumVerticalLine', 'SpectralLine',
            'SliceIndicatorMarks', 'ShadowMixin', 'ShadowLine', 'ShadowLabelFixedY',
            'PluginMark', 'LinesAutoUnit', 'PluginLine', 'PluginScatter',
            'LineAnalysisContinuum', 'LineAnalysisContinuumCenter',
            'LineAnalysisContinuumLeft', 'LineAnalysisContinuumRight',
-           'LineUncertainties', 'ScatterMask', 'SelectedSpaxel', 'MarkersMark', 'FootprintOverlay']
+           'LineUncertainties', 'ScatterMask', 'SelectedSpaxel', 'MarkersMark', 'FootprintOverlay',
+           'ApertureMark', 'SpectralExtractionPreview']
 
 accent_color = "#c75d2c"
 
 
 class OffscreenLinesMarks(HubListener):
     def __init__(self, viewer):
         self.viewer = viewer
@@ -139,37 +140,40 @@
 
 class BaseSpectrumVerticalLine(Lines, PluginMark, HubListener):
     def __init__(self, viewer, x, **kwargs):
         self.viewer = viewer
 
         # the location of the marker will need to update automatically if the
         # underlying data changes (through a unit conversion, for example)
-        viewer.state.add_callback("reference_data",
-                                  self._update_reference_data)
+        if hasattr(viewer.state, 'reference_data'):
+            viewer.state.add_callback("reference_data",
+                                      self._update_reference_data)
 
         scales = viewer.scales
 
         # Lines.__init__ will set self.x
         super().__init__(x=[x, x], y=[0, 1],
                          scales={'x': scales['x'], 'y': LinearScale(min=0, max=1)},
                          **kwargs)
 
     def _update_reference_data(self, reference_data):
         if reference_data is None:
             return
-        self._update_data(reference_data.get_object(cls=Spectrum1D).spectral_axis)
+        self._update_unit(reference_data.get_object(cls=Spectrum1D).spectral_axis.unit)
 
-    def _update_data(self, x_all):
+    def _update_unit(self, new_unit):
         # the x-units may have changed.  We want to convert the internal self.x
         # from self.xunit to the new units (x_all.unit)
-        new_unit = x_all.unit
+        if self.xunit is None:
+            self.xunit = new_unit
+            return
         if new_unit == self.xunit:
             return
         old_quant = self.x[0]*self.xunit
-        x = old_quant.to_value(x_all.unit, equivalencies=u.spectral())
+        x = old_quant.to_value(new_unit, equivalencies=u.spectral())
         self.x = [x, x]
         self.xunit = new_unit
 
 
 class SpectralLine(BaseSpectrumVerticalLine):
     """
     Subclass on bqplot Lines, mostly so that we can erase spectral lines
@@ -244,166 +248,160 @@
 
         self._identify = identify
         self.stroke_width = 3 if identify else 1
 
     def _process_identify_change(self, msg):
         self.identify = msg.name_rest == self.table_index
 
-    def _update_data(self, x_all):
-        new_unit = x_all.unit
+    def _update_unit(self, new_unit):
+        if self.xunit is None:
+            self.xunit = new_unit
+            return
         if new_unit == self.xunit:
             return
 
         old_quant = self._rest_value*self.xunit
         self._rest_value = old_quant.to_value(new_unit, equivalencies=u.spectral())
         # re-compute self.x from current redshift (instead of converting that as well)
         self.redshift = self._redshift
         self.xunit = new_unit
 
 
 class SliceIndicatorMarks(BaseSpectrumVerticalLine, HubListener):
     """Subclass on bqplot Lines to handle slice/wavelength indicator.
     """
-    def __init__(self, viewer, slice=0, **kwargs):
+    def __init__(self, viewer, value=0, **kwargs):
         self._viewer = viewer
+        self._value = None
         self._oob = False  # out-of-bounds, either False, 'left', or 'right'
         self._active = False
+        # TODO: new viewers need to respect plugin settings
         self._show_if_inactive = True
-        self._show_wavelength = True
-
-        self.slice = slice
-        x_all = viewer.data()[0].spectral_axis
-        # _update_data will set self._x_all, self._x_unit, self.x
-        self._update_data(x_all)
+        self._show_value = True
 
-        viewer.state.add_callback("x_min", lambda x_min: self._handle_oob(update_label=True))
-        viewer.state.add_callback("x_max", lambda x_max: self._handle_oob(update_label=True))
+        viewer.state.add_callback("x_min", lambda x_min: self._value_handle_oob(update_label=True))
+        viewer.state.add_callback("x_max", lambda x_max: self._value_handle_oob(update_label=True))
         viewer.session.hub.subscribe(self, SliceToolStateMessage,
                                      handler=self._on_change_state)
 
         super().__init__(viewer=viewer,
-                         x=self.x[0],
+                         x=[value, value],
                          stroke_width=2,
                          marker='diamond',
                          fill='none', close_path=False,
                          labels=['slice'], labels_visibility='none', **kwargs)
 
-        self._handle_oob()
+        self.value = value
 
         # instead of using the Lines label which is limited, we'll use a Label object which
         # will follow the x-coordinate of the slice indicator line, with a fixed y-value
         # (in axes-units) and will flip its alignment depending on whether the line is on the
         # left or right side of the axes.
         self.label = ShadowLabelFixedY(viewer, self, shadow_traits=[], default_size=12, y=0.95)
 
         # default to the initial state of the tool since we can't control if this will
         # happen before or after the initialization of the tool
-        self._on_change_state({'active': True})
+        tool_active = self.viewer.toolbar.active_tool_id == 'jdaviz:selectslice'
+        self._on_change_state({'active': tool_active})
 
     @property
     def marks(self):
         return [self, self.label]
 
-    def _handle_oob(self, x_coord=None, update_label=False):
-        if x_coord is None:
-            x_coord = self._slice_to_x(self.slice)
+    def _value_handle_oob(self, x=None, update_label=False):
+        if x is None:
+            x = self.value
+        else:
+            self._value = x
         x_min, x_max = self._viewer.state.x_min, self._viewer.state.x_max
         if x_min is None or x_max is None:
-            self.x = [x_coord, x_coord]
+            self.x = [x, x]
             return
         x_range = x_max - x_min
         padding_fig = 0.01
         padding = padding_fig * x_range
         x_min += padding
         x_max -= padding
-        if x_coord < x_min:
+        # ensure y-scale has been set (we'll only be overriding x, but scatter viewers complain
+        # if y-scale is not set)
+        self.scales.setdefault('y', LinearScale(min=0, max=1))
+        if x < x_min:
             self.x = [padding_fig, padding_fig]
             self.scales = {**self.scales, 'x': LinearScale(min=0, max=1)}
             self.line_style = 'dashed'
             self._oob = 'left'
-        elif x_coord > x_max:
+        elif x > x_max:
             self.x = [1-padding_fig, 1-padding_fig]
             self.scales = {**self.scales, 'x': LinearScale(min=0, max=1)}
             self.line_style = 'dashed'
             self._oob = 'right'
         else:
-            self.x = [x_coord, x_coord]
+            self.x = [x, x]
             self.scales = {**self.scales, 'x': self._viewer.scales['x']}
             self.line_style = 'solid'
             self._oob = False
         if update_label:
             self._update_label()
 
-    def _slice_to_x(self, slice=0):
-        if not isinstance(slice, int):
-            raise TypeError(f"slice must be of type int, not {type(slice)}")
-        return self._x_all[slice]
-
     def _update_colors_opacities(self):
-        # orange (accent) if active, import button blue otherwise (see css in app.vue)
+        # orange (accent) if active, import button blue otherwise (see css in main_styles.vue)
         if not self._show_if_inactive and not self._active:
             self.label.visible = False
             self.visible = False
             return
 
         self.visible = True
-        self.label.visible = self._show_wavelength
+        self.label.visible = self._show_value
         self.colors = ["#c75109" if self._active else "#007BA1"]
         self.opacities = [1.0 if self._active else 0.9]
 
     def _on_change_state(self, msg={}):
         if isinstance(msg, dict):
             changes = msg
         else:
+            if msg.viewer is not None and msg.viewer != self.viewer:
+                return
             changes = msg.change
 
         for k, v in changes.items():
             if k == 'active':
                 self._active = v
             elif k == 'show_indicator':
                 self._show_if_inactive = v
-            elif k == 'show_wavelength':
-                self._show_wavelength = v
+            elif k == 'show_value':
+                self._show_value = v
 
         self._update_colors_opacities()
 
     def _update_label(self):
+        def _formatted_value(value):
+            power = abs(np.log10(value))
+            if power >= 3:
+                # use scientific notation
+                return f'{value:0.4e}'
+            else:
+                return f'{value:0.4f}'
+
+        valuestr = _formatted_value(self.value)
+        xunit = str(self.xunit) if self.xunit is not None else ''
         # U+00A0 is a blank space, U+25C0 a left arrow triangle, and U+25B6 a right arrow triangle
         if self._oob == 'left':
-            self.labels = [f'\u00A0 \u25c0 {self._slice_to_x(self.slice):0.4e} {self._x_unit} \u00A0']  # noqa
+            self.labels = [f'\u00A0 \u25c0 {valuestr} {xunit} \u00A0']  # noqa
         elif self._oob == 'right':
-            self.labels = [f'{self._slice_to_x(self.slice):0.4e} {self._x_unit} \u25b6 \u00A0']
+            self.labels = [f'{valuestr} {xunit} \u25b6 \u00A0']
         else:
-            self.labels = [f'\u00A0 {self._slice_to_x(self.slice):0.4e} {self._x_unit} \u00A0']
+            self.labels = [f'\u00A0 {valuestr} {xunit} \u00A0']
 
     @property
-    def slice(self):
-        return self._slice
+    def value(self):
+        return self._value
 
-    @slice.setter
-    def slice(self, slice):
-        self._slice = slice
-        # if this is within the init, the data may not have been set yet,
-        # in which case we'll just set self._slice for the first time, but
-        # do not need to update self.x or label (yet)
-        if hasattr(self, '_x_all'):
-            x_coord = self._slice_to_x(slice)
-            self._handle_oob(x_coord)
-            self._update_label()
-
-    def _update_data(self, x_all):
-        # we want to preserve slice number, so we'll do a bit more than the
-        # default unit-conversion in the base class
-        self._x_all = x_all.value
-        self._x_unit = str(x_all.unit)
-        x_coord = self._slice_to_x(self.slice)
-        self._handle_oob(x_coord)
-        if self.labels_visibility == 'label':
-            # update label with new value/unit
-            self._update_label()
+    @value.setter
+    def value(self, value):
+        self._value_handle_oob(value, update_label=True)
 
 
 class ShadowMixin:
     """Mixin class to propagate traits from one mark object to another.
     Anything in ``sync_traits`` will be mirrored directly from
     ``shadowing`` to the shadowed object.
 
@@ -648,14 +646,25 @@
         super().__init__(viewer, **kwargs)
 
     @property
     def overlay(self):
         return self._overlay
 
 
+class ApertureMark(PluginLine):
+    def __init__(self, viewer, id, **kwargs):
+        self._id = id
+        super().__init__(viewer, **kwargs)
+
+
+class SpectralExtractionPreview(PluginLine):
+    def __init__(self, viewer, **kwargs):
+        super().__init__(viewer, **kwargs)
+
+
 class HistogramMark(Lines):
     def __init__(self, min_max_value, scales, **kwargs):
         # Vertical line in LinearScale
         y = [0, 1]
         colors = [accent_color]
         line_style = "solid"
         super().__init__(x=min_max_value, y=y, scales=scales, colors=colors, line_style=line_style,
```

### Comparing `jdaviz-3.8.2/jdaviz/core/region_translators.py` & `jdaviz-3.9.0/jdaviz/core/region_translators.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,34 +16,29 @@
                      CircleAnnulusPixelRegion, CircleAnnulusSkyRegion,
                      EllipseAnnulusPixelRegion, EllipseAnnulusSkyRegion,
                      RectangleAnnulusPixelRegion, RectangleAnnulusSkyRegion, PixCoord)
 
 __all__ = ['regions2roi', 'regions2aperture', 'aperture2regions']
 
 
-def _get_region_from_spatial_subset(plugin_obj, subset_state, dataset=None):
+def _get_region_from_spatial_subset(plugin_obj, subset_state):
     """Convert the given ``glue`` ROI subset state to ``regions`` shape.
 
     .. note:: This is for internal use only in Imviz plugins.
 
     Parameters
     ----------
     plugin_obj : obj
         Plugin instance that needs this translation.
         The plugin is assumed to have a special setup that gives
-        it access to these attributes: ``app`` and ``dataset_selected``.
-        The ``app._jdaviz_helper.get_link_type`` method must also
-        exist.
+        it access to these attributes: ``app`` and ``app._link_type``.
 
     subset_state : obj
         ROI subset state to translate.
 
-    dataset : string, optional
-        Name of the dataset.  If not provided, will look for ``plugin_obj.dataset_selected``.
-
     Returns
     -------
     reg : `regions.Region`
         An equivalent ``regions`` shape. This can be a pixel or sky
         region, so the plugin needs to be able to deal with both.
 
     See Also
@@ -52,20 +47,16 @@
 
     """
     from glue_astronomy.translators.regions import roi_subset_state_to_region
 
     # Subset is defined against its parent. This is not necessarily
     # the current viewer reference data, which can be changed.
 
-    if dataset is None:
-        dataset = plugin_obj.dataset_selected
-
-    # See https://github.com/spacetelescope/jdaviz/issues/2230
-    link_type = plugin_obj.app._jdaviz_helper.get_link_type(
-        subset_state.xatt.parent.label, dataset)
+    # Mixed link types no longer allowed, so just check app setting.
+    link_type = plugin_obj.app._link_type
 
     return roi_subset_state_to_region(subset_state, to_sky=(link_type == 'wcs'))
 
 
 def regions2roi(region_shape, wcs=None):
     """Convert a given ``regions`` shape to ``glue`` ROI.
```

### Comparing `jdaviz-3.8.2/jdaviz/core/registries.py` & `jdaviz-3.9.0/jdaviz/core/registries.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,57 +32,61 @@
     return re.sub("([a-z0-9])([A-Z])", r"\1_\2", s1).lower()
 
 
 class UniqueDictRegistry(DictRegistry):
     """Base registry class that handles hashmap-like associations between a string
     representation of a plugin and the class to be instantiated.
     """
-    def add(self, name, cls):
+    def add(self, name, cls, overwrite=False):
         """Add an item to the registry.
 
         Parameters
         ----------
         name : str
             The name referencing the associated class in the registry.
         cls : type
             The class definition (not instance) associated with the name given
             in the first parameter.
+        overwrite : bool, optional
+            Whether to overwrite an existing entry with the same ``label``.
         """
-        if name in self.members:
+        if name in self.members and not overwrite:
             raise ValueError(f"Viewer with the name {name} already exists, "
-                             f"please choose a different name.")
+                             f"please choose a different name or pass overwrite=True.")
         else:
             self.members[name] = cls
 
 
 class ViewerRegistry(UniqueDictRegistry):
     """Registry containing references to custom viewers."""
-    def __call__(self, name=None, label=None):
+    def __call__(self, name=None, label=None, overwrite=False):
         def decorator(cls):
-            self.add(name, cls, label)
+            self.add(name, cls, label, overwrite=overwrite)
             return cls
         return decorator
 
-    def add(self, name, cls, label=None):
+    def add(self, name, cls, label=None, overwrite=False):
         """Add an item to the registry.
 
         Parameters
         ----------
         name : str
             The key referencing the associated class in the registry
             dictionary.
         cls : type
             The class definition (not instance) associated with the name given
             in the first parameter.
         label : str, optional
             The label displayed in the tooltip when hovering over the tray tab.
+        overwrite : bool, optional
+            Whether to overwrite an existing entry with the same ``label``.
         """
-        if name in self.members:
+        if name in self.members and not overwrite:
             raise ValueError(f"Viewer with the name {name} already exists, "
-                             f"please choose a different name.")
+                             f"please choose a different name or pass overwrite=True.")
         else:
             self.members[name] = {'label': label, 'cls': cls}
 
 
 class TrayRegistry(UniqueDictRegistry):
     """Registry containing references to plugins that will be added to the sidebar
     tray tabs.
@@ -96,30 +100,30 @@
             "cls_attr": f"_default_{_to_snake(category)}_viewer_reference_name",
             "init_kwarg": f"{_to_snake(category)}_viewer_reference_name",
             "require_kwargs": [f"require_{_to_snake(category)}_viewer"]
         } for category in default_viewer_category
     }
 
     def __call__(self, name=None, label=None, icon=None,
-                 viewer_requirements=[]):
+                 viewer_requirements=[], overwrite=False):
         def decorator(cls):
             # The class must inherit from `VuetifyTemplate` in order to be
             # ingestible by the component initialization.
             if not issubclass(cls, VuetifyTemplate):
                 raise ValueError(
                     f"Unrecognized superclass for {cls.__name__}. All "
                     f"registered components must inherit from "
                     f"`ipyvuetify.VuetifyTemplate`.")
 
-            self.add(name, cls, label, icon, viewer_requirements)
+            self.add(name, cls, label, icon, viewer_requirements, overwrite)
             return cls
         return decorator
 
     def add(self, name, cls, label=None, icon=None,
-            viewer_requirements=[]):
+            viewer_requirements=[], overwrite=False):
         """Add an item to the registry.
 
         Parameters
         ----------
         name : str
             The key referencing the associated class in the registry
             dictionary.
@@ -128,18 +132,20 @@
             in the first parameter.
         label : str, optional
             The label displayed in the tooltip when hovering over the tray tab.
         icon : str, optional
             The name of the icon to render in the tray tab.
         viewer_requirements : str, list of str
             Required viewers for this plugin.
+        overwrite : bool, optional
+            Whether to overwrite an existing entry with the same ``label``.
         """
-        if name in self.members:
+        if name in self.members and not overwrite:
             raise ValueError(f"Viewer with the name {name} already exists, "
-                             f"please choose a different name.")
+                             f"please choose a different name or pass overwrite=True.")
         else:
             # store the registry name/label so we can access them from the instantiated
             # objects (when determining if a specific plugin is open, for example)
             viewer_reference_name_kwargs = {}
 
             if not isinstance(viewer_requirements, list):
                 viewer_requirements = [viewer_requirements]
@@ -166,44 +172,44 @@
                                   'viewer_reference_name_kwargs': viewer_reference_name_kwargs}
 
 
 class ToolRegistry(UniqueDictRegistry):
     """Registry containing references to plugins which will populate the
     application-level toolbar.
     """
-    def __call__(self, name=None):
+    def __call__(self, name=None, overwrite=False):
         def decorator(cls):
             # The class must inherit from `Widget` in order to be
             # ingestible by the component initialization.
             if not issubclass(cls, Widget):
                 raise ValueError(
                     f"Unrecognized superclass for `{cls.__name__}`. All "
                     f"registered tools must inherit from "
                     f"`ipywidgets.Widget`.")
 
-            self.add(name, cls)
+            self.add(name, cls, overwrite)
             return cls
         return decorator
 
 
 class MenuRegistry(UniqueDictRegistry):
     """Registry containing references to plugins that will populate the
     application-level menu bar.
     """
-    def __call__(self, name=None):
+    def __call__(self, name=None, overwrite=False):
         def decorator(cls):
             # The class must inherit from `VuetifyTemplate` in order to be
             # ingestible by the component initialization.
             if not issubclass(cls, Widget):
                 raise ValueError(
                     f"Unrecognized superclass for {cls.__name__}. All "
                     f"registered tools must inherit from "
                     f"`ipywidgets.Widget`.")
 
-            self.add(name, cls)
+            self.add(name, cls, overwrite)
             return cls
         return decorator
 
 
 class DataParserRegistry(UniqueDictRegistry):
     """Registry containing parsing functions for attempting to auto-populate the
     application-defined initial viewers.
```

### Comparing `jdaviz-3.8.2/jdaviz/core/template_mixin.py` & `jdaviz-3.9.0/jdaviz/core/template_mixin.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,59 +5,79 @@
 import astropy.units as u
 import bqplot
 from contextlib import contextmanager
 import numpy as np
 import os
 import threading
 import time
+import warnings
 
 from echo import delay_callback
 from functools import cached_property
 from ipyvuetify import VuetifyTemplate
 from glue.config import colormaps
 from glue.core import Data, HubListener
 from glue.core.link_helpers import LinkSame
 from glue.core.message import (DataCollectionAddMessage,
                                DataCollectionDeleteMessage,
                                SubsetCreateMessage,
                                SubsetDeleteMessage,
                                SubsetUpdateMessage)
 from glue.core.roi import CircularAnnulusROI
 from glue_jupyter import jglue
+from glue_jupyter.common.toolbar_vuetify import read_icon
 from glue_jupyter.bqplot.histogram import BqplotHistogramView
 from glue_jupyter.bqplot.image import BqplotImageView
 from glue_jupyter.registries import viewer_registry
 from glue_jupyter.widgets.linked_dropdown import get_choices as _get_glue_choices
+from regions import PixelRegion
 from specutils import Spectrum1D
-from traitlets import Any, Bool, HasTraits, List, Unicode, observe
+from specutils.manipulation import extract_region
+from traitlets import Any, Bool, Dict, Float, HasTraits, List, Unicode, observe
 
 from ipywidgets import widget_serialization
 from ipypopout import PopoutButton
 
 from jdaviz import __version__
 from jdaviz.components.toolbar_nested import NestedJupyterToolbar
+from jdaviz.core.custom_traitlets import FloatHandleEmpty
 from jdaviz.core.events import (AddDataMessage, RemoveDataMessage,
                                 ViewerAddedMessage, ViewerRemovedMessage,
                                 ViewerRenamedMessage, SnackbarMessage,
-                                AddDataToViewerMessage)
-from jdaviz.core.region_translators import _get_region_from_spatial_subset
+                                AddDataToViewerMessage, ChangeRefDataMessage,
+                                PluginTableAddedMessage, PluginTableModifiedMessage,
+                                PluginPlotAddedMessage, PluginPlotModifiedMessage)
+
+from jdaviz.core.marks import (LineAnalysisContinuum,
+                               LineAnalysisContinuumCenter,
+                               LineAnalysisContinuumLeft,
+                               LineAnalysisContinuumRight,
+                               ShadowLine, ApertureMark)
+from jdaviz.core.region_translators import regions2roi, _get_region_from_spatial_subset
+from jdaviz.core.tools import ICON_DIR
 from jdaviz.core.user_api import UserApiWrapper, PluginUserApi
-from jdaviz.utils import get_subset_type
+from jdaviz.style_registry import PopoutStyleWrapper
+from jdaviz.utils import get_subset_type, is_wcs_only, is_not_wcs_only, _wcs_only_label
 
 
 __all__ = ['show_widget', 'TemplateMixin', 'PluginTemplateMixin',
-           'skip_if_no_updates_since_last_active', 'with_spinner',
+           'skip_if_no_updates_since_last_active', 'with_spinner', 'with_temp_disable',
            'ViewerPropertiesMixin',
            'BasePluginComponent',
+           'MultiselectMixin',
            'SelectPluginComponent', 'UnitSelectPluginComponent', 'EditableSelectPluginComponent',
            'PluginSubcomponent',
-           'SubsetSelect', 'SpatialSubsetSelectMixin', 'SpectralSubsetSelectMixin',
-           'DatasetSpectralSubsetValidMixin',
+           'SubsetSelect', 'SubsetSelectMixin',
+           'SpatialSubsetSelectMixin', 'SpectralSubsetSelectMixin',
+           'ApertureSubsetSelect', 'ApertureSubsetSelectMixin',
+           'DatasetSpectralSubsetValidMixin', 'SpectralContinuumMixin',
            'ViewerSelect', 'ViewerSelectMixin',
            'LayerSelect', 'LayerSelectMixin',
+           'PluginTableSelect', 'PluginTableSelectMixin',
+           'PluginPlotSelect', 'PluginPlotSelectMixin',
            'NonFiniteUncertaintyMismatchMixin',
            'DatasetSelect', 'DatasetSelectMixin', 'DatasetMultiSelectMixin',
            'FileImportSelectPluginComponent', 'HasFileImportSelect',
            'Table', 'TableMixin',
            'Plot', 'PlotMixin',
            'AutoTextField', 'AutoTextFieldMixin',
            'AddResults', 'AddResultsMixin',
@@ -172,15 +192,18 @@
         # store references to all bqplot widgets that need to handle resizing
         obj.bqplot_figs_resize = []
 
         return obj
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.popout_button = PopoutButton(self, window_features='popup,width=400,height=600')
+        self.popout_button = PopoutButton(
+            PopoutStyleWrapper(content=self),
+            window_features='popup,width=400,height=600'
+        )
         self._viewer_callbacks = {}
         self.hub.subscribe(self, ViewerRemovedMessage,
                            handler=lambda msg: self._remove_viewer_callbacks(msg.viewer_id))
 
     @property
     def app(self):
         """
@@ -233,14 +256,17 @@
         self._viewer_callbacks = {k: v for k, v in self._viewer_callbacks.items()
                                   if k.split(':')[0] != viewer_id}
 
 
 def skip_if_no_updates_since_last_active(skip_if_not_active=True):
     def decorator(meth):
         def wrapper(self, msg={}):
+            if msg is None:
+                # method was called manually, don't skip
+                return meth(self, msg)
             if isinstance(msg, dict) and msg.get('name', None) == 'is_active':
                 if self.is_active and meth.__name__ in self._methods_skip_since_last_active:
                     # then we haven't received any other messages since the last time the plugin
                     # received an is_active switch, and so we should skip calling the method.
                     return
             elif not self.is_active:
                 # then we've received some other message while the plugin is inactive.
@@ -285,27 +311,64 @@
                 raise
             setattr(self, spinner_traitlet, False)
             return ret_
         return wrapper
     return decorator
 
 
+def with_temp_disable(timeout=0.3,
+                      disable_traitlet='previews_temp_disabled',
+                      time_traitlet='previews_last_time'):
+    """
+    decorator on a plugin method to track the amount of time the wrapped method takes, and disable
+    live plugin-previews if it takes longer than ``timeout`` seconds.  The wrapped method should
+    also observe ``disable_traitlet`` ('previews_temp_disabled', by default).
+
+    This should be used with::
+
+        <plugin-previews-temp-disabled
+          :previews_temp_disabled.sync="previews_temp_disabled"
+          :previews_last_time="previews_last_time"
+          :show_live_preview.sync="show_live_preview"
+        />
+    """
+    def decorator(meth):
+        def wrapper(self, *args, **kwargs):
+            if getattr(self, disable_traitlet):
+                return
+            start = time.time()
+            ret_ = meth(self, *args, **kwargs)
+            exec_time = np.round(time.time() - start, 2)
+            setattr(self, time_traitlet, exec_time)
+            if exec_time > timeout:
+                setattr(self, disable_traitlet, True)
+            return ret_
+        return wrapper
+    return decorator
+
+
 class PluginTemplateMixin(TemplateMixin):
     """
     This base class can be inherited by all sidebar/tray plugins to expose common functionality.
     """
-    disabled_msg = Unicode("").tag(sync=True)
+    disabled_msg = Unicode("").tag(sync=True)  # noqa if non-empty, will show this message in place of plugin content
+    irrelevant_msg = Unicode("").tag(sync=True)  # noqa if non-empty, will exclude from the tray, and show this message in place of any content in other instances
     docs_link = Unicode("").tag(sync=True)  # set to non-empty to override value in vue file
+    docs_description = Unicode("").tag(sync=True)  # set to non-empty to override value in vue file
     plugin_opened = Bool(False).tag(sync=True)  # noqa any instance of the plugin is open (recently sent an "alive" ping)
     uses_active_status = Bool(False).tag(sync=True)  # noqa whether the plugin has live-preview marks, set to True in plugins to expose keep_active switch
     keep_active = Bool(False).tag(sync=True)  # noqa whether the live-preview marks show regardless of active state, inapplicable unless uses_active_status is True
     is_active = Bool(False).tag(sync=True)  # noqa read-only: whether the previews should be shown according to plugin_opened and keep_active
+    scroll_to = Bool(False).tag(sync=True)  # noqa once set to True, vue will scroll to the element and reset to False
     spinner = Bool(False).tag(sync=True)  # noqa use along-side @with_spinner() and <plugin-add-results :action_spinner="spinner">
+    previews_temp_disabled = Bool(False).tag(sync=True)  # noqa use along-side @with_temp_disable() and <plugin-previews-temp-disabled :previews_temp_disabled.sync="previews_temp_disabled" :previews_last_time="previews_last_time" :show_live_preview.sync="show_live_preview"/>
+    previews_last_time = Float(0).tag(sync=True)
 
     def __init__(self, **kwargs):
+        self._plugin_name = kwargs.pop('plugin_name', None)
         self._viewer_callbacks = {}
         # _inactive_thread: thread checking for alive pings to control plugin_opened
         self._inactive_thread = None
         self._ping_timestamp = 0
         # _ping_delay_ms should match value in setTimeout in tray_plugin.vue
         # NOTE: could control with a traitlet, but then would need to pass through each
         # <j-tray-plugin> component
@@ -321,14 +384,22 @@
 
     @property
     def user_api(self):
         # plugins should override this to pass their own list of expose functionality, which
         # can even be dependent on config, etc.
         return PluginUserApi(self, expose=[])
 
+    @observe('irrelevant_msg')
+    def _irrelevant_msg_changed(self, *args):
+        labels = [ti['label'] for ti in self.app.state.tray_items]
+        if self._registry_label not in labels:
+            return
+        index = labels.index(self._registry_label)
+        self.app.state.tray_items[index]['is_relevant'] = len(self.irrelevant_msg) == 0
+
     def vue_plugin_ping(self, ping_timestamp):
         if isinstance(ping_timestamp, dict):
             # popout windows can sometimes ping but send an empty dictionary instead of the
             # timestamp, in that case, let's set the latest ping time to now
             ping_timestamp = time.time() * 1000
         self._ping_timestamp = ping_timestamp
 
@@ -376,23 +447,32 @@
             return lambda data: plugin_method(viewer, data)
 
         key = f'{viewer.reference_id}:{plugin_method.__name__}'
         if key not in self._viewer_callbacks.keys():
             self._viewer_callbacks[key] = plugin_viewer_callback(viewer, plugin_method)
         return self._viewer_callbacks.get(key)
 
-    def open_in_tray(self):
+    def open_in_tray(self, scroll_to=True):
         """
         Open the plugin in the sidebar/tray (and open the sidebar if it is not already).
+
+        Parameters
+        ----------
+        scroll_to : bool, optional
+            Whether to immediately scroll to the plugin opened in the tray.
         """
         app_state = self.app.state
         app_state.drawer = True
         index = [ti['name'] for ti in app_state.tray_items].index(self._registry_name)
         if index not in app_state.tray_items_open:
             app_state.tray_items_open = app_state.tray_items_open + [index]
+        if scroll_to:
+            # sleep 0.5s to ensure plugin is intialized and user can see scrolling
+            time.sleep(0.5)
+            self.scroll_to = True
 
     def close_in_tray(self, close_sidebar=False):
         """
         Close the plugin in the sidebar/tray.
 
         Parameters
         ----------
@@ -401,17 +481,18 @@
         """
         app_state = self.app.state
         index = [ti['name'] for ti in app_state.tray_items].index(self._registry_name)
         app_state.tray_items_open = [ind for ind in app_state.tray_items_open if ind != index]
         if close_sidebar:
             self.app.state.drawer = False
 
-    @observe('plugin_opened', 'keep_active')
+    @observe('plugin_opened', 'keep_active', 'irrelevant_msg')
     def _update_is_active(self, *args):
-        self.is_active = self.keep_active or self.plugin_opened
+        self.is_active = ((len(self.irrelevant_msg) == 0)
+                          and (self.keep_active or self.plugin_opened))
 
     @contextmanager
     def as_active(self):
         """
         Context manager to temporarily enable keep_active and enable live-previews and keypress
         events, even if the plugin UI is not opened.
         """
@@ -471,14 +552,15 @@
 
 class BasePluginComponent(HubListener, ViewerPropertiesMixin):
     """
     This base class handles attaching traitlets from the plugin itself to logic
     handled within the component, support for caching and clearing caches on properties,
     and common properties for accessing the app, etc.
     """
+
     def __init__(self, plugin, **kwargs):
         self._plugin_traitlets = {k: v for k, v in kwargs.items() if v is not None}
         self._plugin = plugin
         self._cached_properties = []
         super().__init__()
 
     def __getattr__(self, attr):
@@ -499,14 +581,20 @@
         """
         if not len(attrs):
             attrs = self._cached_properties
         for attr in attrs:
             if attr in self.__dict__:
                 del self.__dict__[attr]
 
+    def add_traitlets(self, **traitlets):
+        for k, v in traitlets.items():
+            if v is None:
+                continue
+            self._plugin_traitlets[k] = v
+
     def add_observe(self, traitlet_name, handler, first=False):
         self._plugin.observe(handler, traitlet_name)
         if first:
             # re-order the callbacks so this one is first
             existing_callbacks = self._plugin._trait_notifiers[traitlet_name]['change']
             new_order = [handler] + [other for other in existing_callbacks if other != handler]
             self._plugin._trait_notifiers[traitlet_name]['change'] = new_order
@@ -548,14 +636,20 @@
             return d
 
         return [_dict_from_viewer(viewer, self.app._viewer_item_by_id(vid))
                 for vid, viewer in self.app._viewer_store.items()
                 if viewer.__class__.__name__ != 'MosvizTableViewer']
 
 
+class MultiselectMixin(VuetifyTemplate):
+    icon_radialtocheck = Unicode(read_icon(os.path.join(ICON_DIR, 'radialtocheck.svg'), 'svg+xml')).tag(sync=True)  # noqa
+    icon_checktoradial = Unicode(read_icon(os.path.join(ICON_DIR, 'checktoradial.svg'), 'svg+xml')).tag(sync=True)  # noqa
+    multiselect = Bool(False).tag(sync=True)
+
+
 class SelectPluginComponent(BasePluginComponent, HasTraits):
     """
     Plugin select, with support for single or multi-selection.
 
     Useful API methods/attributes:
 
     * :meth:`choices`
@@ -882,14 +976,15 @@
         :from_file="from_file"
         :from_file_message.sync="from_file_message"
         @click-cancel="method_selected=method_items[0].label"
         @click-import="file_import_accept()">
           <g-file-import id="file-uploader"></g-file-import>
       </plugin-file-import>
     """
+
     def __init__(self, plugin, **kwargs):
         self._cached_obj = {}
 
         if "From File..." not in kwargs['manual_options']:
             kwargs['manual_options'] += ['From File...']
 
         if not isinstance(plugin, HasFileImportSelect):  # pragma: no cover
@@ -1036,14 +1131,15 @@
         :edit_value.sync="edit_value"
         :items="items"
         :selected.sync="selected"
         label="Label"
         hint="Select an item to modify."
       </plugin-editable-select>
     """
+
     def __init__(self, *args, **kwargs):
         """
         Parameters
         ----------
         plugin
             the parent plugin object
         items : str
@@ -1077,14 +1173,15 @@
         self._name = kwargs.get('name', 'entry')  # used for error messages
         self._on_add = kwargs.get('on_add', lambda *args: None)
         self._on_add_after_selection = kwargs.get('on_add_after_selection', lambda *args: None)
         self._on_rename = kwargs.get('on_rename', lambda *args: None)
         self._on_rename_after_selection = kwargs.get('on_rename_after_selection', lambda *args: None)  # noqa
         self._on_remove = kwargs.get('on_remove', lambda *args: None)
         self._on_remove_after_selection = kwargs.get('on_remove_after_selection', lambda *args: None)  # noqa
+        self._validate_choice = kwargs.get('validate_choice', lambda *args: '')
 
     def _multiselect_changed(self):
         # already subscribed to traitlet by SelectPluginComponent
         if self.multiselect:
             raise ValueError("EditableSelectPluginComponent does not support multiselect")
 
     def _selected_changed(self, event):
@@ -1121,14 +1218,17 @@
         self.items = [{"label": opt} for opt in self._manual_options]
 
     def _check_new_choice(self, label):
         if not len(label):
             raise ValueError("new choice must not be blank")
         if label in self.choices:
             raise ValueError(f"'{label}' is already a valid choice")
+        validate_err = self._validate_choice(label)
+        if len(validate_err):
+            raise ValueError(f"'{label}' is not valid: {validate_err}")
 
     def add_choice(self, label, set_as_selected=True):
         """
         Add a new entry/choice.
 
         Parameters
         ----------
@@ -1218,32 +1318,35 @@
 
     To use in a plugin:
 
     * create (empty) traitlets in the plugin
     * register with all the automatic logic in the plugin's init by passing the string names
       of the respective traitlets.
     * use component in plugin template (see below)
-    * refer to properties above based on the interally stored reference to the
+    * refer to properties above based on the internally stored reference to the
       instantiated object of this component
     * observe the traitlets created and defined in the plugin, as necessary
 
     Example template (label and hint are optional)::
 
       <plugin-layer-select
         :items="layer_items"
         :selected.sync="layer_selected"
         :show_if_single_entry="true"
         label="Layer"
         hint="Select layer."
       />
     """
+
     def __init__(self, plugin, items, selected, viewer,
                  multiselect=None,
                  default_text=None, manual_options=[],
-                 default_mode='first'):
+                 default_mode='first',
+                 filters=['not_child_layer'],
+                 only_wcs_layers=False):
         """
         Parameters
         ----------
         plugin
             the parent plugin object
         items : str
             the name of the items traitlet defined in ``plugin``
@@ -1251,18 +1354,21 @@
             the name of the selected traitlet defined in ``plugin``
         viewer: str
             the name of the traitlet defined in ``plugin`` storing the viewer(s) to expose the
             layers
         default_text : str or None
             the text to show for no selection.  If not provided or None, no entry will be provided
             in the dropdown for no selection.
-        manual_options: list
+        manual_options : list
             list of options to provide that are not automatically populated by subsets.  If
             ``default`` text is provided but not in ``manual_options`` it will still be included as
             the first item in the list.
+        default_mode : str, optional
+            What mode to use when making the default selection.  Valid options: first, default_text,
+            empty.
         """
         super().__init__(plugin,
                          items=items,
                          selected=selected,
                          viewer=viewer,
                          multiselect=multiselect,
                          default_text=default_text,
@@ -1283,14 +1389,15 @@
         self.hub.subscribe(self, SubsetDeleteMessage,
                            handler=lambda _: self._update_layer_items())
 
         self.app.state.add_callback('layer_icons', self._update_layer_items)
         self.add_observe(viewer, self._on_viewer_selected_changed)
         self.add_observe(selected, self._update_layer_items)
         self._update_layer_items()
+        self.update_wcs_only_filter(only_wcs_layers)
 
     def _get_viewer(self, viewer):
         # newer will likely be the viewer name in most cases, but viewer id in the case
         # of additional viewers in imviz.
         try:
             return self.app.get_viewer(viewer)
         except TypeError:
@@ -1299,21 +1406,28 @@
     @property
     def viewer_objs(self):
         viewer_names = self.viewer
         if not isinstance(viewer_names, list):
             viewer_names = [viewer_names]
         return [self._get_viewer(viewer) for viewer in viewer_names]
 
+    def _is_valid_item(self, lyr):
+        def not_child_layer(lyr):
+            # ignore layers that are children in associations:
+            return self.app._get_assoc_data_parent(lyr.label) is None
+
+        return super()._is_valid_item(lyr, locals())
+
     def _layer_to_dict(self, layer_label):
         is_subset = None
         colors = []
         visibilities = []
         for viewer in self.viewer_objs:
             for layer in viewer.layers:
-                if layer.layer.label == layer_label:
+                if layer.layer.label == layer_label and is_not_wcs_only(layer.layer):
                     if is_subset is None:
                         is_subset = ((hasattr(layer, 'state') and hasattr(layer.state, 'subset_state')) or  # noqa
                                      (hasattr(layer, 'layer') and hasattr(layer.layer, 'subset_state')))  # noqa
 
                     if (getattr(viewer.state, 'color_mode', None) == 'Colormaps'
                             and hasattr(layer.state, 'cmap')):
                         colors.append(layer.state.cmap.name)
@@ -1346,14 +1460,16 @@
                 old_viewer = self._get_viewer(old_viewer)
                 if old_viewer is None:
                     continue
                 # NOTE: color_mode callback must be conflicting with something else, so instead
                 # we call _update_layer_items in the PlotOptionsSyncState for color_mode
                 # old_viewer.state.remove_callback('color_mode', self._update_layer_items)
                 for layer in old_viewer.state.layers:
+                    if is_wcs_only(layer.layer):
+                        continue
                     layer.remove_callback('color', self._update_layer_items)
                     if hasattr(layer, 'cmap'):
                         layer.remove_callback('cmap', self._update_layer_items)
                     if hasattr(layer, 'bitmap_visible'):
                         layer.remove_callback('bitmap_visible', self._update_layer_items)
                     elif hasattr(layer, 'visible'):
                         layer.remove_callback('visible', self._update_layer_items)
@@ -1362,43 +1478,45 @@
                 new_viewer = self._get_viewer(new_viewer)
                 if new_viewer is None:
                     continue
                 # NOTE: color_mode callback must be conflicting with something else, so instead
                 # we call _update_layer_items in the PlotOptionsSyncState for color_mode
                 # new_viewer.state.add_callback('color_mode', self._update_layer_items)
                 for layer in new_viewer.state.layers:
+                    if is_wcs_only(layer.layer):
+                        continue
                     layer.add_callback('color', self._update_layer_items)
                     if hasattr(layer, 'cmap'):
                         layer.add_callback('cmap', self._update_layer_items)
                     if hasattr(layer, 'bitmap_visible'):
                         layer.add_callback('bitmap_visible', self._update_layer_items)
                     if hasattr(layer, 'visible'):
                         layer.add_callback('visible', self._update_layer_items)
 
     def _on_subset_created(self, msg=None):
         new_subset_label = self.app.data_collection.subset_groups[-1].label
         viewer = self.viewer if isinstance(self.viewer, list) else [self.viewer]
         for current_viewer in viewer:
             for layer in self._get_viewer(current_viewer).state.layers:
-                if layer.layer.label == new_subset_label:
-                    # Is it ok if only one subset layer has this callback?
+                if layer.layer.label == new_subset_label and is_not_wcs_only(layer.layer):
                     layer.add_callback('color', self._update_layer_items)
                     layer.add_callback('visible', self._update_layer_items)
-                    break
                     # TODO: Add ability to add new item to self.items instead of recompiling
         self._update_layer_items({'source': 'subset_added'})
 
     def _on_data_added(self, msg=None):
         if msg is None or not hasattr(msg, 'data') or msg.data is None:
             return
         new_data_label = msg.data.label
         viewer = self.viewer if isinstance(self.viewer, list) else [self.viewer]
         for current_viewer in viewer:
             for layer in self._get_viewer(current_viewer).state.layers:
                 if layer.layer.label == new_data_label and not hasattr(layer.layer, 'subset_state'):
+                    if is_wcs_only(layer.layer):
+                        continue
                     # Add a callback to the layer's color attribute to call
                     # _on_layers_changed whenever the color changes
                     # TODO: find out if this conflicts with another color change event
                     #  and is causing the lag in the color picker
                     layer.add_callback('color', self._update_layer_items)
                     if hasattr(layer, 'cmap'):
                         layer.add_callback('cmap', self._update_layer_items)
@@ -1410,46 +1528,85 @@
         self._update_layer_items({'source': 'data_added'})
 
     @observe('filters')
     def _update_layer_items(self, msg={}):
         # NOTE: _on_layers_changed is passed without a msg object during init
         # TODO: Handle changes to just one item without recompiling the whole thing
         manual_items = [{'label': label} for label in self.manual_options]
-        all_layers = [layer for viewer in self.viewer_objs
-                      for layer in getattr(viewer, 'layers', [])]
+        # use getattr so the super() call above doesn't try to access the attr before
+        # it is initialized:
+
+        all_layers = [
+            layer for viewer in self.viewer_objs
+            for layer in getattr(viewer, 'layers', [])
+            if self._is_valid_item(layer.layer)
+        ]
+
         # remove duplicates - we'll loop back through all selected viewers to get a list of colors
         # and visibilities later within _layer_to_dict
-        layer_labels = [layer.layer.label for layer in all_layers if self.app.state.layer_icons.get(layer.layer.label)]  # noqa
+        layer_labels = [
+            layer.layer.label for layer in all_layers
+            if self.app.state.layer_icons.get(layer.layer.label) or
+            self.only_wcs_layers
+        ]
         unique_layer_labels = list(set(layer_labels))
-
         layer_items = [self._layer_to_dict(layer_label) for layer_label in unique_layer_labels]
 
         def _sort_by_icon(items_dict):
-            return items_dict['icon']
+            icon = items_dict['icon']
+            return icon if icon is not None else ''
+
         layer_items.sort(key=_sort_by_icon)
 
         self.items = manual_items + layer_items
 
         self._apply_default_selection()
 
+    def update_wcs_only_filter(self, wcs_only):
+        """
+        The layers that are populated in LayerSelect.choices
+        will be either WCS-only layers (for setting viewer orientation)
+        or non-WCS-only layers (for "real data"). This method toggles
+        the layer choices by adjusting the layer filters on this
+        LayerSelect instance.
+
+        Parameters
+        ----------
+        wcs_only : bool
+            `True` will filter only the WCS-only layers, `False` will
+            give the non-WCS-only layers.
+        """
+
+        filter_names = [getattr(filt, '__name__', '') for filt in self.filters]
+
+        if not wcs_only and 'is_wcs_only' in filter_names:
+            self.filters.remove(*[filt for filt in self.filters
+                                  if getattr(filt, '__name__', '') == 'is_wcs_only'])
+        elif wcs_only and 'is_wcs_only' not in filter_names:
+            self.add_filter(is_wcs_only)
+
+    @property
+    def only_wcs_layers(self):
+        return 'is_wcs_only' in [getattr(filt, '__name__', '') for filt in self.filters]
+
     @cached_property
     def selected_obj(self):
         viewer_names = self.viewer
         if not isinstance(viewer_names, list):
             # case for single-select on the viewer select
             viewer_names = [viewer_names]
 
         selected = self.selected
         if not isinstance(selected, list):
             selected = [selected]
 
         viewers = [self._get_viewer(viewer_name) for viewer_name in viewer_names]
 
         layers = [[layer for layer in viewer.layers
-                   if layer.layer.label in selected]
+                   if layer.layer.label in selected and self._is_valid_item(layer.layer)]
                   for viewer in viewers]
 
         if not self.is_multiselect and len(layers) == 1:
             return layers[0]
         else:
             return layers
 
@@ -1503,17 +1660,15 @@
     * :meth:`~SelectPluginComponent.is_multiselect`
     * :meth:`~SelectPluginComponent.select_default`
     * :meth:`~SelectPluginComponent.select_all` (only if ``is_multiselect``)
     * :meth:`~SelectPluginComponent.select_none` (only if ``is_multiselect``)
     * :attr:`selected_obj`
     * :attr:`selected_subset_state`
     * :meth:`selected_min_max`
-    """
 
-    """
     Traitlets (in the object, custom traitlets in the plugin):
 
     * ``items`` (list of dicts with keys: label, color, type)
     * ``selected`` (string)
     * ``selected_has_subregions`` (bool, OPTIONAL)
 
     Properties (in the object only):
@@ -1563,25 +1718,28 @@
             the name of the traitlet defining whether the dropdown should accept multiple selections
         selected_has_subregions : str
             the name of the selected_has_subregions traitlet defined in ``plugin``, optional
         dataset : str
             the name of the dataset traitlet defined in ``plugin``, to be used for accessing how
             the subset is applied to the data (masks, etc), optional
         viewers : list
-            the reference names or ids of the viewer to extract the subregion.  If not provided o
+            the reference names or ids of the viewer to extract the subregion.  If not provided or
             None, will loop through all references.
         default_text : str or None
             the text to show for no selection.  If not provided or None, no entry will be provided
             in the dropdown for no selection.
         manual_options : list
             list of options to provide that are not automatically populated by subsets.  If
             ``default`` text is provided but not in ``manual_options`` it will still be included as
             the first item in the list.
         filters : list
             list of strings (for built-in filters) or callables to filter to only valid options.
+        default_mode : str, optional
+            What mode to use when making the default selection.  Valid options: first, default_text,
+            empty.
         """
         super().__init__(plugin,
                          items=items,
                          selected=selected,
                          multiselect=multiselect,
                          filters=filters,
                          selected_has_subregions=selected_has_subregions,
@@ -1612,15 +1770,16 @@
             self._update_subset(lyr)
 
     def _selected_changed(self, event):
         super()._selected_changed(event)
         self._update_has_subregions()
 
     def _on_dataset_selected_changed(self, event):
-        self._clear_cache('selected_subset_mask', 'selected_spatial_region')
+        self._clear_cache('selected_subset_mask',
+                          'selected_spatial_region')
 
     def _subset_to_dict(self, subset):
         # find layer artist in default spectrum-viewer
         for viewer in self.viewers:
             for layer in viewer.layers:
                 if layer.layer.label == subset.label:
                     color = layer.state.color
@@ -1754,32 +1913,30 @@
 
     def _get_spatial_region(self, dataset, subset=None):
         if subset is None:
             subset = self.selected
             subset_state = self.selected_subset_state
         else:
             subset_state = self._get_subset_state(subset)
-        region = _get_region_from_spatial_subset(self.plugin,
-                                                 subset_state,
-                                                 dataset=dataset)
+        if subset_state is None:
+            return None
+        region = _get_region_from_spatial_subset(self.plugin, subset_state)
         region.meta['label'] = subset
         return region
 
     @cached_property
     def selected_spatial_region(self):
         if not getattr(self, 'dataset', None):  # pragma: no cover
             raise ValueError("Retrieving subset mask requires associated dataset")
         if self.is_multiselect and self.dataset.is_multiselect:  # pragma: no cover
-            # technically this could work if either has length of one, but would require extra
-            # logic
             raise NotImplementedError("cannot access selected_spatial_region for multiple subsets and multiple datasets")  # noqa
         types = self.selected_item.get('type')
         if not isinstance(types, list):
             types = [types]
-        if np.any([type != 'spatial' for type in types]):
+        if np.any([type not in ('spatial', None) for type in types]):
             raise TypeError("This action is only supported on spatial-type subsets")
         if self.is_multiselect:
             return [self._get_spatial_region(dataset=self.dataset.selected, subset=subset) for subset in self.selected]  # noqa
         return self._get_spatial_region(dataset=self.dataset.selected)
 
     def selected_min_max(self, dataset):
         """
@@ -1794,14 +1951,50 @@
             return np.nanmin(dataset.spectral_axis), np.nanmax(dataset.spectral_axis)
         if self.selected_item.get('type') != 'spectral':
             raise TypeError("This action is only supported on spectral-type subsets")
         else:
             return self.selected_obj.lower, self.selected_obj.upper
 
 
+class SubsetSelectMixin(VuetifyTemplate, HubListener):
+    """
+    Applies the SubsetSelect component as a mixin in the base plugin.  This
+    automatically adds traitlets as well as new properties to the plugin with minimal
+    extra code.  For multiple instances or custom traitlet names/defaults, use the
+    component instead.
+
+    To use in a plugin:
+
+    * add ``SubsetSelectMixin`` as a mixin to the class
+    * use the traitlets available from the plugin or properties/methods available from
+      ``plugin.subset``.
+
+    Example template (label and hint are optional)::
+
+      <plugin-subset-select
+        :items="subset_items"
+        :selected.sync="subset_selected"
+        :show_if_single_entry="true"
+        label="Subset"
+        hint="Select subset."
+      />
+
+    """
+    subset_items = List().tag(sync=True)
+    subset_selected = Any().tag(sync=True)
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.subset = SubsetSelect(self,
+                                   'subset_items',
+                                   'subset_selected',
+                                   dataset='dataset' if hasattr(self, 'dataset') else None,
+                                   multiselect='multiselect' if hasattr(self, 'multiselect') else None)  # noqa
+
+
 class SpectralSubsetSelectMixin(VuetifyTemplate, HubListener):
     """
     Applies the SubsetSelect component as a mixin in the base plugin.  This
     automatically adds traitlets as well as new properties to the plugin with minimal
     extra code.  For multiple instances or custom traitlet names/defaults, use the
     component instead.
 
@@ -1873,14 +2066,554 @@
                                            'spatial_subset_selected',
                                            'spatial_subset_selected_has_subregions',
                                            dataset='dataset' if hasattr(self, 'dataset') else None,
                                            default_text='Entire Cube',
                                            filters=['is_spatial'])
 
 
+class ApertureSubsetSelect(SubsetSelect):
+    """
+    Plugin select for aperture subsets, with support for single or multi-selection, as well as
+    live-preview rendered in the viewers.
+
+    Useful API methods/attributes:
+
+    * :meth:`~SelectPluginComponent.choices`
+    * ``selected``
+    * :meth:`~SelectPluginComponent.is_multiselect`
+    * :meth:`~SelectPluginComponent.select_default`
+    * :meth:`~SelectPluginComponent.select_all` (only if ``is_multiselect``)
+    * :meth:`~SelectPluginComponent.select_none` (only if ``is_multiselect``)
+    * :attr:`~SubsetSelect.selected_obj`
+    * :attr:`~SubsetSelect.selected_subset_state`
+    * :meth:`~SubsetSelect.selected_min_max`
+    * :meth:`marks`
+    * :meth:`image_viewers`
+
+    Traitlets (in the object, custom traitlets in the plugin):
+
+    * ``items`` (list of dicts with keys: label, color, type)
+    * ``selected`` (string)
+    * ``selected_validity`` (dict)
+
+    Properties (in the object only):
+
+    * ``labels`` (list of labels corresponding to items)
+    * ``selected_item`` (dictionary in ``items`` coresponding to ``selected``, cached)
+    * ``selected_obj`` (subset object corresponding to ``selected``, cached)
+    * ``marks`` (list of marks added to image viewers in the app to preview the apertures)
+
+    Methods (in the object only):
+
+    * ``selected_min_max(cube)`` (quantity, only applicable for spectral subsets)
+
+    To use in a plugin:
+
+    * create (empty) traitlets in the plugin
+    * register with all the automatic logic in the plugin's init by passing the string names
+      of the respective traitlets.
+    * use component in plugin template (see below)
+    * refer to properties above based on the interally stored reference to the
+      instantiated object of this component
+    * observe the traitlets created and defined in the plugin, as necessary
+
+    Example template (label and hint are optional)::
+
+      <plugin-subset-select
+        :items="aperture_items"
+        :selected.sync="aperture_selected"
+        :show_if_single_entry="true"
+        label="Aperture"
+        hint="Select aperture."
+      />
+
+    """
+    def __init__(self, plugin, items, selected, selected_validity,
+                 scale_factor, multiselect=None,
+                 dataset=None, viewers=None, default_text=None):
+        """
+        Parameters
+        ----------
+        plugin
+            the parent plugin object
+        items : str
+            the name of the items traitlet defined in ``plugin``
+        selected : str
+            the name of the selected traitlet defined in ``plugin``
+        selected_validity: str
+            the name of the selected validity dict traitlet defined in ``plugin``
+        scale_factor : str
+            the name of the traitlet defining the radius factor for the drawn aperture
+        multiselect : str
+            the name of the traitlet defining whether the dropdown should accept multiple selections
+        dataset : str
+            the name of the dataset traitlet defined in ``plugin``, to be used for accessing how
+            the subset is applied to the data (masks, etc), optional
+        viewers : list
+            the reference names or ids of the viewer to extract the subregion.  If not provided or
+            None, will loop through all references.
+        """
+        # NOTE: is_not_composite is assumed in _get_mark_coords_and_validate
+        super().__init__(plugin,
+                         items=items,
+                         selected=selected,
+                         multiselect=multiselect,
+                         filters=['is_spatial'],
+                         dataset=dataset,
+                         viewers=viewers,
+                         default_text=default_text)
+
+        self.add_traitlets(selected_validity=selected_validity,
+                           scale_factor=scale_factor)
+
+        self.add_observe('is_active', self._plugin_active_changed)
+        self.add_observe(selected, self._update_mark_coords)
+        self.add_observe(scale_factor, self._update_mark_coords)
+        # add marks to any new viewers
+        self.hub.subscribe(self, ViewerAddedMessage, handler=self._update_mark_coords)
+        # update coordinates when reference data is changed
+        # NOTE: when link type is changed, all subsets are required to be dropped
+        self.hub.subscribe(self, ChangeRefDataMessage, handler=self._update_mark_coords)
+
+    def _update_subset(self, *args, **kwargs):
+        # update coordinates when subset is modified (with subset tools plugin or drag event)
+        super()._update_subset(*args, **kwargs)
+        self._update_mark_coords()
+
+    def _on_dataset_selected_changed(self, event):
+        super()._on_dataset_selected_changed(event)
+        self._update_mark_coords()
+
+    def _set_mark_visiblities(self, visible):
+        for mark in self.marks:
+            mark.visible = visible
+
+    def _plugin_active_changed(self, *args):
+        self._set_mark_visiblities(self.plugin.is_active)
+
+    @property
+    def image_viewers(self):
+        return [viewer for viewer in self.app._viewer_store.values()
+                if isinstance(viewer, BqplotImageView)]
+
+    @property
+    def marks(self):
+        all_aperture_marks = []
+        for viewer in self.image_viewers:
+            # search for existing mark
+            matches = [mark for mark in viewer.figure.marks
+                       if (isinstance(mark, ApertureMark) and
+                           mark._id == self._plugin_traitlets['selected'])]
+            if len(matches):
+                all_aperture_marks += matches
+                continue
+
+            x_coords, y_coords, self.selected_validity = self._get_mark_coords_and_validate(viewer)
+
+            mark = ApertureMark(
+                viewer,
+                id=self._plugin_traitlets['selected'],
+                x=x_coords,
+                y=y_coords,
+                colors=['#c75109'],
+                fill_opacities=[0.0],
+                visible=self.plugin.is_active)
+            all_aperture_marks.append(mark)
+            viewer.figure.marks = viewer.figure.marks + [mark]
+        return all_aperture_marks
+
+    def _get_mark_coords_and_validate(self, viewer=None, selected=None):
+        multiselect = getattr(self, 'multiselect', False)
+
+        if viewer is None:
+            viewer = self.app._jdaviz_helper.default_viewer._obj
+        if selected is None:
+            selected = self.selected
+            objs = self.selected_obj if multiselect else [self.selected_obj]
+        else:
+            objs = self._get_selected_obj(selected)
+            if isinstance(selected, str):
+                selected = [selected]
+                objs = [objs]
+
+        if not len(selected) or not len(self.dataset.selected):
+            validity = {'is_aperture': False,
+                        'aperture_message': 'no subset selected'}
+            return [], [], validity
+        if selected in self._manual_options:
+            validity = {'is_aperture': False,
+                        'aperture_message': 'no subset selected'}
+            return [], [], validity
+
+        # if any of the selected entries are composite, then _get_spatial_region
+        # (or selected_spatial_region) will fail.
+        if np.any([len(obj) > 1 for obj in objs]):
+            validity = {'is_aperture': False,
+                        'aperture_message': 'composite subsets are not supported',
+                        'is_composite': True}
+            return [], [], validity
+
+        if multiselect or selected != self.selected:
+            # assume first dataset (for retrieving the region object)
+            # but iterate over all subsets
+            spatial_regions = [self._get_spatial_region(dataset=self.dataset.selected[0], subset=subset)  # noqa
+                               for subset in selected if subset != self._manual_options]
+        else:
+            # use cached version
+            spatial_regions = [self.selected_spatial_region]
+
+        x_coords, y_coords = np.array([]), np.array([])
+        for spatial_region in spatial_regions:
+            if spatial_region is None:
+                continue
+
+            if isinstance(spatial_region, PixelRegion):
+                pixel_region = spatial_region
+            else:
+                wcs = getattr(viewer.state.reference_data, 'coords', None)
+                if wcs is None:
+                    validity = {'is_aperture': False,
+                                'aperture_message': 'invalid wcs'}
+                    return [], [], validity
+                pixel_region = spatial_region.to_pixel(wcs)
+            roi = regions2roi(pixel_region)
+
+            # NOTE: this assumes that we'll apply the same radius factor to all subsets (all will
+            # be defined at the same slice for cones in cubes)
+#            if self.scale_factor == 1.0:  # this would catch annulus, which might cause confusion
+#                pass
+            if hasattr(roi, 'radius'):
+                roi.radius *= self.scale_factor
+            elif hasattr(roi, 'radius_x'):
+                roi.radius_x *= self.scale_factor
+                roi.radius_y *= self.scale_factor
+            elif hasattr(roi, 'center') and hasattr(roi, 'xmin') and hasattr(roi, 'xmax'):
+                center = roi.center()
+                half_width = abs(roi.xmax - roi.xmin) * 0.5 * self.scale_factor
+                half_height = abs(roi.ymax - roi.ymin) * 0.5 * self.scale_factor
+                roi.xmin = center[0] - half_width
+                roi.xmax = center[0] + half_width
+                roi.ymin = center[1] - half_height
+                roi.ymax = center[1] + half_height
+            elif isinstance(roi, CircularAnnulusROI):
+                validity = {'is_aperture': False,
+                            'aperture_message': 'annulus is not a supported aperture'}
+                return [], [], validity
+            else:  # pragma: no cover
+                # known unsupported shapes: annulus
+                # TODO: specific case for annulus
+                validity = {'is_aperture': False,
+                            'aperture_message': 'shape does not support scale factor'}
+                return [], [], validity
+
+            if hasattr(roi, 'to_polygon'):
+                x, y = roi.to_polygon()
+
+                # concatenate with nan between to avoid line connecting separate subsets
+                x_coords = np.concatenate((x_coords, np.array([np.nan]), x))
+                y_coords = np.concatenate((y_coords, np.array([np.nan]), y))
+            else:
+                validity = {'is_aperture': False,
+                            'aperture_message': 'could not convert roi to polygon'}
+                return [], [], validity
+
+        validity = {'is_aperture': True}
+        return x_coords, y_coords, validity
+
+    def _update_mark_coords(self, *args):
+        for viewer in self.image_viewers:
+            x_coords, y_coords, self.selected_validity = self._get_mark_coords_and_validate(viewer)
+            for mark in self.marks:
+                if mark.viewer != viewer:
+                    continue
+                mark.x, mark.y = x_coords, y_coords
+
+
+class ApertureSubsetSelectMixin(VuetifyTemplate, HubListener):
+    """
+    Applies the ApertureSubsetSelect component as a mixin in the base plugin.  This
+    automatically adds traitlets as well as new properties to the plugin with minimal
+    extra code.  For multiple instances or custom traitlet names/defaults, use the
+    component instead.
+
+    To use in a plugin:
+
+    * add ``ApertureSubsetSelectMixin`` as a mixin to the class BEFORE ``DatasetSelectMixin``
+    * use the traitlets available from the plugin or properties/methods available from
+      ``plugin.aperture``.
+
+    Example template (label and hint are optional)::
+
+      <plugin-subset-select
+        :items="aperture_items"
+        :selected.sync="aperture_selected"
+        label="Aperture"
+        hint="Select aperture."
+      />
+
+    """
+    aperture_items = List([]).tag(sync=True)
+    aperture_selected = Any('').tag(sync=True)
+    aperture_selected_validity = Dict().tag(sync=True)
+    aperture_scale_factor = Float(1).tag(sync=True)
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.aperture = ApertureSubsetSelect(self,
+                                             'aperture_items',
+                                             'aperture_selected',
+                                             'aperture_selected_validity',
+                                             'aperture_scale_factor',
+                                             dataset='dataset' if hasattr(self, 'dataset') else None,  # noqa
+                                             multiselect='multiselect' if hasattr(self, 'multiselect') else None)  # noqa
+
+
+class PluginTableSelect(SelectPluginComponent):
+    """
+    Plugin select for plugin table entries, with support for single or multi-selection.
+
+    Useful API methods/attributes:
+
+    * :meth:`~SelectPluginComponent.choices`
+    * ``selected``
+    * :attr:`selected_obj`
+    * :meth:`~SelectPluginComponent.is_multiselect`
+    * :meth:`~SelectPluginComponent.select_default`
+    * :meth:`~SelectPluginComponent.select_all` (only if ``is_multiselect``)
+    * :meth:`~SelectPluginComponent.select_none` (only if ``is_multiselect``)
+
+    Traitlets (in the object, custom traitlets in the plugin):
+
+    * ``items`` (list of dicts with keys: label)
+    * ``selected`` (string)
+
+    Properties (in the object only):
+
+    * ``selected_obj``
+
+    Methods (in the object only):
+
+    * ``get_object``
+
+    To use in a plugin:
+
+    * create traitlets with default values
+    * register with all the automatic logic in the plugin's init by passing the string names
+      of the respective traitlets
+    * use component in plugin template (see below)
+    * refer to properties above based on the interally stored reference to the
+      instantiated object of this component
+
+    Example template (label and hint are optional)::
+
+      <v-select
+        :items="table_items"
+        :selected.sync="table_selected"
+        label="Table"
+        hint="Select table."
+      />
+    """
+
+    def __init__(self, plugin, items, selected,
+                 multiselect=None,
+                 filters=['not_empty_table'],
+                 default_text=None, manual_options=[],
+                 default_mode='first'):
+        """
+        Parameters
+        ----------
+        plugin
+            the parent plugin object
+        items : str
+            the name of the items traitlet defined in ``plugin``
+        selected : str
+            the name of the selected traitlet defined in ``plugin``
+        multiselect : str
+            the name of the traitlet defining whether the dropdown should accept multiple selections
+        filters : list
+            list of strings (for built-in filters) or callables to filter to only valid options.
+        default_text : str or None
+            the text to show for no selection.  If not provided or None, no entry will be provided
+            in the dropdown for no selection.
+        manual_options: list
+            list of options to provide that are not automatically populated by datasets.  If
+            ``default`` text is provided but not in ``manual_options`` it will still be included as
+            the first item in the list.
+        default_mode : str, optional
+            What mode to use when making the default selection.  Valid options: first, default_text,
+            empty.
+        """
+        super().__init__(plugin, items=items, selected=selected,
+                         multiselect=multiselect, filters=filters,
+                         default_text=default_text, manual_options=manual_options,
+                         default_mode=default_mode)
+        self.hub.subscribe(self, PluginTableAddedMessage, handler=self._on_tables_changed)
+        self.hub.subscribe(self, PluginTableModifiedMessage, handler=self._on_tables_changed)
+        self._on_tables_changed()
+
+    @observe('filters')
+    def _on_tables_changed(self, *args):
+        manual_items = [{'label': label} for label in self.manual_options]
+        self.items = manual_items + [{'label': k} for k, v in self.plugin.app._plugin_tables.items()
+                                     if self._is_valid_item(v._obj)]
+        self._apply_default_selection()
+        # future improvement: only clear cache if the selected data entry was changed?
+        self._clear_cache(*self._cached_properties)
+
+    @cached_property
+    def selected_obj(self):
+        return self.plugin.app._jdaviz_helper.plugin_tables.get(self.selected)
+
+    def _is_valid_item(self, table):
+        def not_empty_table(table):
+            return len(table.items) > 0
+
+        return super()._is_valid_item(table, locals())
+
+
+class PluginTableSelectMixin(VuetifyTemplate, HubListener):
+    plugin_table_items = List().tag(sync=True)
+    plugin_table_selected = Any().tag(sync=True)
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.plugin_table = PluginTableSelect(self,
+                                              'plugin_table_items',
+                                              'plugin_table_selected',
+                                              multiselect='multiselect' if hasattr(self, 'multiselect') else None)  # noqa
+
+
+class PluginPlotSelect(SelectPluginComponent):
+    """
+    Plugin select for plugin plot entries, with support for single or multi-selection.
+
+    Useful API methods/attributes:
+
+    * :meth:`~SelectPluginComponent.choices`
+    * ``selected``
+    * :attr:`selected_obj`
+    * :meth:`~SelectPluginComponent.is_multiselect`
+    * :meth:`~SelectPluginComponent.select_default`
+    * :meth:`~SelectPluginComponent.select_all` (only if ``is_multiselect``)
+    * :meth:`~SelectPluginComponent.select_none` (only if ``is_multiselect``)
+
+    Traitlets (in the object, custom traitlets in the plugin):
+
+    * ``items`` (list of dicts with keys: label)
+    * ``selected`` (string)
+
+    Properties (in the object only):
+
+    * ``selected_obj``
+
+    Methods (in the object only):
+
+    * ``get_object``
+
+    To use in a plugin:
+
+    * create traitlets with default values
+    * register with all the automatic logic in the plugin's init by passing the string names
+      of the respective traitlets
+    * use component in plugin template (see below)
+    * refer to properties above based on the interally stored reference to the
+      instantiated object of this component
+
+    Example template (label and hint are optional)::
+
+      <v-select
+        :items="plot_items"
+        :selected.sync="plot_selected"
+        label="Plot"
+        hint="Select plot."
+      />
+    """
+
+    def __init__(self, plugin, items, selected,
+                 multiselect=None,
+                 filters=['not_empty_plot'],
+                 default_text=None, manual_options=[],
+                 default_mode='first'):
+        """
+        Parameters
+        ----------
+        plugin
+            the parent plugin object
+        items : str
+            the name of the items traitlet defined in ``plugin``
+        selected : str
+            the name of the selected traitlet defined in ``plugin``
+        multiselect : str
+            the name of the traitlet defining whether the dropdown should accept multiple selections
+        filters : list
+            list of strings (for built-in filters) or callables to filter to only valid options.
+        default_text : str or None
+            the text to show for no selection.  If not provided or None, no entry will be provided
+            in the dropdown for no selection.
+        manual_options: list
+            list of options to provide that are not automatically populated by datasets.  If
+            ``default`` text is provided but not in ``manual_options`` it will still be included as
+            the first item in the list.
+        default_mode : str, optional
+            What mode to use when making the default selection.  Valid options: first, default_text,
+            empty.
+        """
+        super().__init__(plugin, items=items, selected=selected,
+                         multiselect=multiselect, filters=filters,
+                         default_text=default_text, manual_options=manual_options,
+                         default_mode=default_mode)
+        self.hub.subscribe(self, PluginPlotAddedMessage, handler=self._on_plots_changed)
+        self.hub.subscribe(self, PluginPlotModifiedMessage, handler=self._on_plots_changed)
+        self._on_plots_changed()
+
+    @observe('filters')
+    def _on_plots_changed(self, *args):
+        manual_items = [{'label': label} for label in self.manual_options]
+        self.items = manual_items + [{'label': k} for k, v in self.plugin.app._plugin_plots.items()
+                                     if self._is_valid_item(v._obj)]
+        self._apply_default_selection()
+        # future improvement: only clear cache if the selected data entry was changed?
+        self._clear_cache(*self._cached_properties)
+
+    @cached_property
+    def selected_obj(self):
+        return self.plugin.app._jdaviz_helper.plugin_plots.get(self.selected)
+
+    def _is_valid_item(self, plot):
+
+        def not_empty_plot(plot):
+            # checks plot.figure.marks to determine if figure is of an empty plot
+            # not sure if this is a foolproof way to do this?
+            return len(plot.figure.marks) > 0
+
+        return super()._is_valid_item(plot, locals())
+
+
+class PluginPlotSelectMixin(VuetifyTemplate, HubListener):
+    plugin_plot_items = List().tag(sync=True)
+    plugin_plot_selected = Any().tag(sync=True)
+    plugin_plot_selected_widget = Any().tag(sync=True)
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.plugin_plot = PluginPlotSelect(self,
+                                            'plugin_plot_items',
+                                            'plugin_plot_selected',
+                                            multiselect='multiselect' if hasattr(self, 'multiselect') else None)  # noqa
+
+    @observe('plugin_plot_selected')
+    def _plugin_plot_selected_changed(self, *args):
+        if not hasattr(self, 'plugin_plot'):
+            return
+        if self.plugin_plot_selected == '':
+            self.plugin_plot_selected_widget = ''
+        else:
+            self.plugin_plot_selected_widget = f'IPY_MODEL_{self.plugin_plot.selected_obj._obj.model_id}'  # noqa
+
+
 class DatasetSpectralSubsetValidMixin(VuetifyTemplate, HubListener):
     """
     Adds a traitlet tracking whether self.dataset and self.spectral_subset
     overlap in the spectral axis.
 
     Note that if using in another method that is also observing dataset_selected
     or spectral_subset_selected, that that method could be called before the traitlet
@@ -1971,31 +2704,237 @@
         mismatch = np.any(np.logical_and(~np.isfinite(uncert), np.isfinite(flux)))
 
         # np.any returns numpy bool type, which traitlets doesn't like
         # so cast to boolean
         self.non_finite_uncertainty_mismatch = bool(mismatch)
 
 
+class SpectralContinuumMixin(VuetifyTemplate, HubListener):
+    """
+    Plugin select to choose options for a linear spectral continuum.
+    """
+    continuum_subset_items = List().tag(sync=True)
+    continuum_subset_selected = Unicode().tag(sync=True)
+
+    continuum_width = FloatHandleEmpty(3).tag(sync=True)
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.continuum = SubsetSelect(self,
+                                      'continuum_subset_items',
+                                      'continuum_subset_selected',
+                                      manual_options=['None', 'Surrounding'],
+                                      default_mode='first',
+                                      filters=['is_spectral'])
+
+    def _continuum_remove_none_option(self):
+        self.continuum.items = [item for item in self.continuum.items
+                                if item['label'] != 'None']
+        self.continuum._apply_default_selection()
+
+    @property
+    def continuum_marks(self):
+        marks = {}
+        viewer = self.app.get_viewer(self._default_spectrum_viewer_reference_name)
+        if viewer is None:
+            return {}
+        for mark in viewer.figure.marks:
+            if isinstance(mark, LineAnalysisContinuum):
+                # NOTE: we don't use isinstance anymore because of nested inheritance
+                if mark.__class__.__name__ == 'LineAnalysisContinuumLeft':
+                    marks['left'] = mark
+                elif mark.__class__.__name__ == 'LineAnalysisContinuumCenter':
+                    marks['center'] = mark
+                elif mark.__class__.__name__ == 'LineAnalysisContinuumRight':
+                    marks['right'] = mark
+
+        if not len(marks):
+            if not viewer.state.reference_data:
+                # we don't have data yet for scales, defer initializing
+                return {}
+            # then haven't been initialized yet, so initialize with empty
+            # marks that will be populated once the first analysis is done.
+            marks = {'left': LineAnalysisContinuumLeft(viewer, visible=self.is_active),
+                     'center': LineAnalysisContinuumCenter(viewer, visible=self.is_active),
+                     'right': LineAnalysisContinuumRight(viewer, visible=self.is_active)}
+            shadows = [ShadowLine(mark, shadow_width=2) for mark in marks.values()]
+            # NOTE: += won't trigger the figure to notice new marks
+            viewer.figure.marks = viewer.figure.marks + shadows + list(marks.values())
+
+        return marks
+
+    def _update_continuum_marks(self, mark_x={}, mark_y={}):
+        for pos, mark in self.continuum_marks.items():
+            mark.update_xy(mark_x.get(pos, []), mark_y.get(pos, []))
+
+    def _get_continuum(self, dataset, spatial_subset, spectral_subset, update_marks=False):
+        if dataset.selected == '':
+            self._update_continuum_marks()
+            return None, None, None
+
+        if spatial_subset == 'per-pixel':
+            if self.app.config != 'cubeviz':
+                raise ValueError("per-pixel only supported for cubeviz")
+            full_spectrum = self.dataset.selected_obj
+        else:
+            full_spectrum = dataset.selected_spectrum_for_spatial_subset(spatial_subset.selected if spatial_subset is not None else None,  # noqa
+                                                                         use_display_units=True)
+
+        if full_spectrum is None or self.continuum_width == "":
+            self._update_continuum_marks()
+            return None, None, None
+
+        spectral_axis = full_spectrum.spectral_axis
+        if spectral_axis.unit == u.pix:
+            # plugin should be disabled so not get this far, but can still get here
+            # before the disabled message is set
+            self._update_continuum_marks()
+            return None, None, None
+
+        if self.continuum_subset_selected == spectral_subset.selected:
+            # already raised a validation error in the UI
+            self._update_continuum_marks()
+            return None, None, None
+
+        if spectral_subset.selected == "Entire Spectrum":
+            spectrum = full_spectrum
+        else:
+            sr = self.app.get_subsets(spectral_subset.selected,
+                                      simplify_spectral=True,
+                                      use_display_units=True)
+            spectrum = extract_region(full_spectrum, sr, return_single_spectrum=True)
+            sr_lower = np.nanmin(spectrum.spectral_axis[spectrum.spectral_axis.value >= sr.lower.value])  # noqa
+            sr_upper = np.nanmax(spectrum.spectral_axis[spectrum.spectral_axis.value <= sr.upper.value])  # noqa
+
+        if self.continuum_subset_selected == 'None':
+            self._update_continuum_marks()
+            return spectrum, np.zeros_like(spectrum.flux.value), spectrum
+
+        # compute continuum
+        if self.continuum_subset_selected == "Surrounding" and spectral_subset.selected == "Entire Spectrum": # noqa
+            # we know we'll just use the endpoints, so let's be efficient and not even
+            # try extracting from the region
+            continuum_mask = np.array([0, len(spectral_axis)-1])
+            if update_marks:
+                mark_x = {'left': np.array([]),
+                          'center': np.array([min(spectral_axis.value),
+                                              max(spectral_axis.value)]),
+                          'right': np.array([])}
+
+        elif self.continuum_subset_selected == "Surrounding":
+            # self.spectral_subset_selected != "Entire Spectrum"
+            if self.continuum_width > 10 or self.continuum_width < 1:
+                # DEV NOTE: if changing the limits, make sure to also update the form validation
+                # rules in line_analysis.vue
+                self._update_continuum_marks()
+                return None, None, None
+
+            spectral_region_width = sr_upper - sr_lower
+            # convert width from total relative width, to width per "side"
+            width = (self.continuum_width - 1) / 2
+            left, = np.where((spectral_axis < sr_lower) &
+                             (spectral_axis > sr_lower - spectral_region_width*width))
+            if not len(left):
+                # then no points matching the width are available outside the line region,
+                # so we'll default to the left-most point of the line region.
+                left, = np.where(spectral_axis == min(spectrum.spectral_axis))
+
+            right, = np.where((spectral_axis > sr_upper) &
+                              (spectral_axis < sr_upper + spectral_region_width*width))
+            if not len(right):
+                # then no points matching the width are available outside the line region,
+                # so we'll default to the right-most point of the line region.
+                right, = np.where(spectral_axis == max(spectrum.spectral_axis))
+
+            continuum_mask = np.concatenate((left, right))
+            if update_marks:
+                mark_x = {'left': np.array([min(spectral_axis.value[continuum_mask]),
+                                            sr_lower.value]),
+                          'center': np.array([sr_lower.value,
+                                              sr_upper.value]),
+                          'right': np.array([sr_upper.value,
+                                             max(spectral_axis.value[continuum_mask])])}
+
+        else:
+            # we'll access the mask of the continuum and then apply that to the spectrum.  For a
+            # spatially-collapsed spectrum in cubeviz, this will access the mask from the full
+            # cube, but still apply that to the spatially-collapsed spectrum.
+            continuum_mask = ~self._specviz_helper.get_data(
+                dataset.selected,
+                spectral_subset=self.continuum_subset_selected,
+                use_display_units=False).mask
+            spectral_axis_nanmasked = spectral_axis.value.copy()
+            spectral_axis_nanmasked[~continuum_mask] = np.nan
+            if not update_marks:
+                pass
+            elif spectral_subset.selected == "Entire Spectrum":
+                mark_x = {'left': spectral_axis_nanmasked,
+                          'center': spectral_axis.value,
+                          'right': []}
+            else:
+                mark_x = {'left': spectral_axis_nanmasked[spectral_axis.value < sr_lower.value],
+                          'right': spectral_axis_nanmasked[spectral_axis.value > sr_upper.value]}
+                # Center should extend (at least) across the line region between the full
+                # range defined by the continuum subset(s).
+                # OK for mark_x to be all NaNs.
+                with warnings.catch_warnings():
+                    warnings.simplefilter('ignore', category=RuntimeWarning)
+                    mark_x_min = np.nanmin(mark_x['left'])
+                    mark_x_max = np.nanmax(mark_x['right'])
+                left_min = np.nanmin([mark_x_min, sr_lower.value])
+                right_max = np.nanmax([mark_x_max, sr_upper.value])
+                mark_x['center'] = np.array([left_min, right_max])
+
+        continuum_x = spectral_axis[continuum_mask].value
+        min_x = min(spectral_axis.value)
+        if spatial_subset == 'per-pixel':
+            # full_spectrum.flux is a cube, so we want to act on all spaxels independently
+            continuum_y = full_spectrum.flux[:, :, continuum_mask].value
+
+            def fit_continuum(continuum_y_spaxel):
+                return np.polyfit(continuum_x-min_x, continuum_y_spaxel, deg=1)
+
+            # compute the linear fit for each spaxel independently, along the spectral axis
+            slopes_intercepts = np.apply_along_axis(fit_continuum, 2, continuum_y)
+            slopes = slopes_intercepts[:, :, 0]
+            intercepts = slopes_intercepts[:, :, 1]
+
+            # spectrum.spectral_axis is an array, but we need our continuum to have the same
+            # shape as the fluxes in the cube, so let's just duplicate to the correct shape
+            spectral_axis_cube = np.zeros(spectrum.flux.shape)
+            spectral_axis_cube[:, :] = spectrum.spectral_axis.value
+
+            continuum = slopes[:, :, np.newaxis] * (spectral_axis_cube-min_x) + intercepts[:, :, np.newaxis]  # noqa
+        else:
+            continuum_y = full_spectrum.flux[continuum_mask].value
+            slope, intercept = np.polyfit(continuum_x-min_x, continuum_y, deg=1)
+            continuum = slope * (spectrum.spectral_axis.value-min_x) + intercept
+
+        if update_marks:
+            mark_y = {k: slope * (v-min_x) + intercept for k, v in mark_x.items()}
+            self._update_continuum_marks(mark_x, mark_y)
+
+        return spectrum, continuum, spectrum - continuum
+
+
 class ViewerSelect(SelectPluginComponent):
     """
     Plugin select for viewers, with support for single or multi-selection.
 
     Useful API methods/attributes:
 
     * :meth:`~SelectPluginComponent.choices`
     * ``selected``
     * :attr:`selected_id`
     * :attr:`selected_obj`
     * :meth:`~SelectPluginComponent.is_multiselect`
     * :meth:`~SelectPluginComponent.select_default`
     * :meth:`~SelectPluginComponent.select_all` (only if ``is_multiselect``)
     * :meth:`~SelectPluginComponent.select_none` (only if ``is_multiselect``)
-    """
 
-    """
     Traitlets (in the object, custom traitlets in the plugin):
 
     * ``items`` (list of dicts with keys: id, reference, label)
     * ``selected`` (string)
 
     Properties (in the object only):
 
@@ -2023,14 +2962,15 @@
         :items="viewer_items"
         :selected.sync="viewer_selected"
         label="Viewer"
         hint="Select viewer."
       />
 
     """
+
     def __init__(self, plugin, items, selected,
                  multiselect=None,
                  default_text=None, manual_options=[], default_mode='first'):
         super().__init__(plugin, items=items, selected=selected,
                          multiselect=multiselect,
                          default_text=default_text, manual_options=manual_options,
                          default_mode=default_mode)
@@ -2062,14 +3002,16 @@
         # will allow access to the underlying item/object for any observes in the meantime.
         for item in self.items:
             if item['id'] == selected:
                 return item
 
     @property
     def selected_id(self):
+        if self.selected_item is None:
+            return None
         return self.selected_item.get('id', None)
 
     @property
     def selected_reference(self):
         return self.selected_item.get('reference', None)
 
     def _get_selected_obj(self, selected, selected_id):
@@ -2131,15 +3073,15 @@
     @observe('filters')
     def _on_viewers_changed(self, msg=None):
         # NOTE: _on_viewers_changed is passed without a msg object during init
         # list of dictionaries with id, ref, ref_or_id
         was_empty = len(self.items) == 0
         manual_items = [{'label': label} for label in self.manual_options]
         self.items = manual_items + [{k: v for k, v in vd.items() if k != 'viewer'}
-                                     for vd in self.viewer_dicts if self._is_valid_item(vd['viewer'])] # noqa
+                                     for vd in self.viewer_dicts if self._is_valid_item(vd['viewer'])]  # noqa
         self._apply_default_selection(skip_if_current_valid=not was_empty)
 
 
 class ViewerSelectMixin(VuetifyTemplate, HubListener):
     """
     Applies the ViewerSelect component as a mixin in the base plugin.  This
     automatically adds traitlets as well as new properties to the plugin with minimal
@@ -2181,17 +3123,15 @@
     * ``selected``
     * :attr:`selected_obj`
     * :attr:`selected_dc_item`
     * :meth:`~SelectPluginComponent.is_multiselect`
     * :meth:`~SelectPluginComponent.select_default`
     * :meth:`~SelectPluginComponent.select_all` (only if ``is_multiselect``)
     * :meth:`~SelectPluginComponent.select_none` (only if ``is_multiselect``)
-    """
 
-    """
     Traitlets (in the object, custom traitlets in the plugin):
 
     * ``items`` (list of dicts with keys: label)
     * ``selected`` (string)
 
     Properties (in the object only):
 
@@ -2218,17 +3158,19 @@
         :items="dataset_items"
         :selected.sync="dataset_selected"
         label="Data"
         hint="Select data."
       />
 
     """
+
     def __init__(self, plugin, items, selected,
                  multiselect=None,
-                 filters=['not_from_plugin_model_fitting', 'layer_in_viewers'],
+                 filters=['not_from_plugin_model_fitting', 'layer_in_viewers',
+                          'is_not_wcs_only', 'not_child_layer'],
                  default_text=None, manual_options=[],
                  default_mode='first'):
         """
         Parameters
         ----------
         plugin
             the parent plugin object
@@ -2332,14 +3274,17 @@
         if spatial_subset == SPATIAL_DEFAULT_TEXT:
             spatial_subset = None
         return self.plugin._specviz_helper.get_data(data_label=self.selected,
                                                     spatial_subset=spatial_subset,
                                                     use_display_units=use_display_units)
 
     def _is_valid_item(self, data):
+        def from_plugin(data):
+            return data.meta.get('Plugin', None) is not None
+
         def not_from_plugin(data):
             return data.meta.get('Plugin', None) is None
 
         def not_from_this_plugin(data):
             return data.meta.get('Plugin', None) != self.plugin.__class__.__name__
 
         def not_from_plugin_model_fitting(data):
@@ -2349,15 +3294,15 @@
             return hasattr(data, 'meta') and isinstance(data.meta, dict) and len(data.meta)
 
         def layer_in_viewers(data):
             if not len(self.app.get_viewer_reference_names()):
                 # then this is a bar Application object, so ignore this filter
                 return True
             for viewer in self.viewers:
-                if data.label in [l.layer.label for l in viewer.layers]: # noqa E741
+                if data.label in [l.layer.label for l in viewer.layers]:  # noqa E741
                     return True
             return False
 
         def layer_in_spectrum_viewer(data):
             if not len(self.app.get_viewer_reference_names()):
                 # then this is a bare Application object, so ignore this filter
                 return True
@@ -2377,14 +3322,21 @@
 
         def is_image(data):
             return len(data.shape) == 2
 
         def is_cube(data):
             return len(data.shape) == 3
 
+        def is_not_wcs_only(data):
+            return not data.meta.get(_wcs_only_label, False)
+
+        def not_child_layer(data):
+            # ignore layers that are children in associations:
+            return self.app._get_assoc_data_parent(data.label) is None
+
         return super()._is_valid_item(data, locals())
 
     @observe('filters')
     def _on_data_changed(self, msg=None):
         # NOTE: _on_data_changed is passed without a msg object during init
         # future improvement: don't recreate the entire list when msg is passed
         def _dc_to_dict(data):
@@ -2503,14 +3455,15 @@
         :default="comp_label_default"
         :auto.sync="comp_label_auto"
         :invalid_msg="invalid_msg"
         hint="Label hint."
       ></plugin-auto-label>
 
     """
+
     def __init__(self, plugin, value, default, auto,
                  invalid_msg):
         super().__init__(plugin, value=value,
                          default=default, auto=auto,
                          invalid_msg=invalid_msg)
 
         self.add_observe(default, self._on_set_to_default)
@@ -2618,14 +3571,15 @@
         :add_to_viewer_selected.sync="add_to_viewer_selected"
         action_label="Apply"
         action_tooltip="Apply the action to the data"
         @click:action="apply"
       ></plugin-add-results>
 
     """
+
     def __init__(self, plugin, label, label_default, label_auto,
                  label_invalid_msg, label_overwrite,
                  add_to_viewer_items, add_to_viewer_selected,
                  label_whitelist_overwrite=[]):
         super().__init__(plugin, label=label,
                          label_default=label_default, label_auto=label_auto,
                          label_invalid_msg=label_invalid_msg, label_overwrite=label_overwrite,
@@ -2847,14 +3801,15 @@
 
     * ``value``: the currently set value sent to the underlying ``linked_states`` objects in glue
     * ``text``: the user-friendly equivalent of the currently set value (only when has ``choices``)
     * :meth:`choices` (only when applicable)
     * :attr:`linked_states`
     * :meth:`unmix_state`
     """
+
     def __init__(self, plugin, viewer_select, layer_select, glue_name,
                  value, sync, spinner=None, state_filter=None):
         super().__init__(plugin, value=value, sync=sync)
         self._state_filter = state_filter
         self._linked_states = []
         self._spinner = spinner
         self._processing_change_from_glue = False
@@ -2957,14 +3912,16 @@
 
         # subscribed states can still be nested list
         return viewer_states + layer_states
 
     @cached_property
     def subscribed_icons(self):
         # dictionary items giving information about the entries in subscribed_states
+        if self._viewer_select.selected_item is None:
+            return []
         viewer_icons = self._viewer_select.selected_item.get('icon', [])
         if not isinstance(viewer_icons, list):
             viewer_icons = [viewer_icons]
 
         layer_icons = self._layer_select.selected_item.get('icon', [])
         if not isinstance(layer_icons, list):
             layer_icons = [layer_icons]
@@ -2986,14 +3943,16 @@
             # Set to lower() so that all linked states of a subset
             # (data in viewer with this subset applied) have matching color values
             return str(getattr(state, glue_name)).lower()
         if glue_name in ('contour_visible', 'bitmap_visible'):
             # return False if the layer itself is not visible.  Setting this object
             # to True will then set both glue_name and visible to True.
             return getattr(state, glue_name) and getattr(state, 'visible')
+        if glue_name in ('c_min', 'c_max'):
+            return float(getattr(state, glue_name))
 
         return getattr(state, glue_name)
 
     def _get_glue_choices(self, state):
         glue_name = self.glue_name(state)
         if glue_name == 'cmap':
             return [{'text': cmap[0], 'value': cmap[1].name} for cmap in colormaps.members]
@@ -3057,28 +4016,63 @@
                     glue_name == 'cmap_att'
                 ):
                     # then we can access and populate/update the choices.
                     self.sync = {**self.sync, 'choices': self._get_glue_choices(state)}
         self.sync = {**self.sync,
                      'in_subscribed_states': in_subscribed_states,
                      'icons': icons,
-                     'mixed': len(np.unique(current_glue_values, axis=0)) > 1}
-
-        if len(current_glue_values):
+                     'mixed': self.is_mixed(current_glue_values)}
+        if len(current_glue_values) and current_glue_values[0] is not None:
             # sync the initial value of the widget, avoiding recursion
             self._on_glue_value_changed(current_glue_values[0])
 
+    def is_mixed(self, glue_values):
+        if len(glue_values) and isinstance(glue_values[0], dict):
+            if len(np.unique([len(item) for item in glue_values], axis=0)) > 1:
+                # different lengths
+                return True
+
+            # guaranteed to have same lengths
+            if len(np.unique([list(item.keys()) for item in glue_values], axis=0)) > 1:
+                # different keys
+                return True
+
+            # guaranteed to each have the same set of keys, so now we can loop over keys and
+            # compare values
+            for k in glue_values[0].keys():
+                if len(np.unique([item.get(k) for item in glue_values], axis=0)) > 1:
+                    return True
+
+            return False
+
+        # Need this for temporary None value during startup
+        elif len(glue_values):
+            no_nones = [x for x in glue_values if x is not None]
+            if len(no_nones) == 0:
+                return False
+            if len(no_nones) != len(glue_values):
+                return True
+
+        return len(np.unique(glue_values, axis=0)) > 1
+
     def _update_mixed_state(self):
         if len(self.linked_states) <= 1:
             mixed = False
         else:
             current_glue_values = []
             for state in self.linked_states:
                 current_glue_values.append(self._get_glue_value(state))
-                mixed = len(np.unique(current_glue_values, axis=0)) > 1
+            mixed = self.is_mixed(current_glue_values)
+            # ensure the value corresponds to the first entry, this prevents the case where a glue
+            # change to one of the linked_states changes the value that will be adopted when
+            # unmixing something in mixed state and results in more consistent and predictable
+            # behavior
+            self._processing_change_from_glue = True
+            self.value = current_glue_values[0]
+            self._processing_change_from_glue = False
         self.sync = {**self.sync,
                      'mixed': mixed}
 
     def _on_value_changed(self, msg):
         if self._processing_change_from_glue:
             return
 
@@ -3095,14 +4089,19 @@
                         cmap = member[1]
                         break
                 setattr(glue_state, glue_name, cmap)
             elif glue_name in GLUE_STATES_WITH_HELPERS:
                 helper = getattr(glue_state, f'{glue_name}_helper')
                 value = [choice for choice in helper.choices if str(choice) == msg['new']][0]
                 setattr(glue_state, glue_name, value)
+            elif glue_name in ('zoom_level') and msg['new'] <= 0:
+                # ignore if negative number (otherwise would fail)
+                self.value = msg['old']
+                self._processing_change_to_glue = False
+                return
             else:
                 setattr(glue_state, glue_name, msg['new'])
 
             if glue_name in ['bitmap_visible', 'contour_visible'] and msg['new'] is True:
                 # ensure that the layer is also visible
                 if not glue_state.visible:
                     setattr(glue_state, 'visible', msg['new'])
@@ -3143,21 +4142,28 @@
             return
 
         self._processing_change_from_glue = True
         if "Colormap" in value.__class__.__name__:
             value = value.name
         elif self._glue_name in GLUE_STATES_WITH_HELPERS:
             value = str(value)
-        elif isinstance(self.value, (int, float)) and self._glue_name != 'percentile':
+        elif self._glue_name != 'percentile' and isinstance(self.value, (int, float)):
             # glue might pass us ints for float or vice versa, but our traitlets care
             # so let's cast to the type expected by the traitlet to avoid having to
             # use Any traitlets for all of these.  We skip percentile as that needs
             # to be an Any traitlet in order to handle "Custom"
             value = type(self.value)(value)
         self.value = value
+
+        if self._glue_name == 'stretch_parameters':
+            # stretch_parameters is a dictionary so won't trigger the @observe on
+            # _update_stretch_curve, so we'll need to manually call it (and make sure
+            # it is not skipped if it has already been called since an actual traitlet change)
+            self.plugin._update_stretch_curve()
+
         # need to recompute mixed state
         self._update_mixed_state()
         self._processing_change_from_glue = False
 
     def unmix_state(self, new_value=None):
         if new_value is None:
             new_value = self.value
@@ -3172,15 +4178,18 @@
 class PluginSubcomponent(VuetifyTemplate):
     popout_button = Any().tag(sync=True, **widget_serialization)
 
     def __init__(self, plugin, component_type='table', *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._plugin = plugin
         self._component_type = component_type
-        self.popout_button = PopoutButton(self, window_features='popup,width=800,height=300')
+        self.popout_button = PopoutButton(
+            PopoutStyleWrapper(content=self),
+            window_features='popup,width=800,height=300'
+        )
 
     @property
     def display_name(self):
         return f'{self._plugin._plugin_name}: {self._component_type}'
 
     def vue_popout(self, data=None):
         self.show(loc='popout')
@@ -3253,18 +4262,25 @@
 
     _default_values_by_colname = {}
 
     headers_visible = List([]).tag(sync=True)  # list of strings
     headers_avail = List([]).tag(sync=True)   # list of strings
     items = List().tag(sync=True)  # list of dictionaries, pass single dict to add_row
 
-    def __init__(self, plugin, *args, **kwargs):
+    def __init__(self, plugin, name='table', *args, **kwargs):
         self._qtable = None
+        self._table_name = name
         super().__init__(plugin, 'Table', *args, **kwargs)
 
+        plugin.session.hub.broadcast(PluginTableAddedMessage(sender=self))
+
+    @property
+    def user_api(self):
+        return UserApiWrapper(self, ('clear_table', 'export_table'))
+
     def default_value_for_column(self, colname=None, value=None):
         if colname in self._default_values_by_colname:
             return self._default_values_by_colname.get(colname)
         if isinstance(value, (tuple, list)):
             return [self.default_value_for_column(value=v) for v in value]
         if isinstance(value, (float, int)):
             return np.nan
@@ -3343,34 +4359,46 @@
         missing_headers = [k for k in item.keys() if k not in self.headers_avail]
         if len(missing_headers):
             self.headers_avail = self.headers_avail + missing_headers
             self.headers_visible = self.headers_visible + [m for m in missing_headers if self._new_col_visible(m)]  # noqa
 
         # clean data to show in the UI
         self.items = self.items + [{k: json_safe(k, v) for k, v in item.items()}]
+        self._plugin.session.hub.broadcast(PluginTableAddedMessage(sender=self))
 
     def __len__(self):
         return len(self.items)
 
     def clear_table(self):
         """
         Clear all entries/markers from the current table.
         """
         self.items = []
         self._qtable = None
+        self._plugin.session.hub.broadcast(PluginTableModifiedMessage(sender=self))
 
     def vue_clear_table(self, data=None):
         # if the plugin (or via the TableMixin) has its own clear_table implementation,
         # call that, otherwise call the one defined here
         getattr(self._plugin, 'clear_table', self.clear_table)()
 
-    def export_table(self):
+    def export_table(self, filename=None, overwrite=False):
         """
         Export the QTable representation of the table.
+
+        Parameters
+        ----------
+        filename : str, optional
+            If provided, will write to the file, otherwise will just return the QTable
+            object.
+        overwrite : bool, optional
+            If ``filename`` already exists, should it be overwritten.
         """
+        if filename is not None:
+            self._qtable.write(filename, overwrite=overwrite)
         # TODO: default to only showing selected columns?
         return self._qtable
 
 
 class TableMixin(VuetifyTemplate, HubListener):
     """
     Table subcomponent mixin.
@@ -3385,33 +4413,41 @@
       <jupyter-widget :widget="table_widget"></jupyter-widget>
 
     """
     table_widget = Unicode().tag(sync=True)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.table = Table(self)
+        self.table = Table(self, name='table')
         self.table_widget = 'IPY_MODEL_'+self.table.model_id
 
     def clear_table(self):
         """
         Clear all entries/markers from the current table.
         """
         self.table.clear_table()
 
     def vue_clear_table(self, data=None):
         # call clear_table directly in case the class overloads that method
         # (to also clear markers, etc)
         self.clear_table()
 
-    def export_table(self):
+    def export_table(self, filename=None, overwrite=False):
         """
         Export the QTable representation of the table.
+
+        Parameters
+        ----------
+        filename : str, optional
+            If provided, will write to the file, otherwise will just return the QTable
+            object.
+        overwrite : bool, optional
+            If ``filename`` already exists, should it be overwritten.
         """
-        return self.table.export_table()
+        return self.table.export_table(filename=filename, overwrite=overwrite)
 
 
 class Plot(PluginSubcomponent):
     """
     Plot subcomponent.  For most cases where a plugin only requires a single plot, use the mixin
     instead.
 
@@ -3424,23 +4460,25 @@
 
     """
     template_file = __file__, "../components/plugin_plot.vue"
 
     figure = Any().tag(sync=True, **widget_serialization)
     toolbar = Any().tag(sync=True, **widget_serialization)
 
-    def __init__(self, plugin, viewer_type='scatter', app=None, *args, **kwargs):
+    def __init__(self, plugin, name='plot', viewer_type='scatter', app=None, *args, **kwargs):
         super().__init__(plugin, 'Plot', *args, **kwargs)
         if app is None:
             app = jglue()
 
         self._app = app
         self._plugin = plugin
+        self._plot_name = name
         self.viewer = app.new_data_viewer(viewer_type, show=False)
         self.viewer._plugin = plugin
+        self.viewer._plot = self
         self._viewer_type = viewer_type
         if viewer_type == 'histogram':
             self._viewer_components = ('x',)
         else:
             self._viewer_components = ('x', 'y')
         self.figure = self.viewer.figure
         self._marks = {}
@@ -3451,18 +4489,25 @@
         self.tools_nested = [
                         ['jdaviz:homezoom', 'jdaviz:prevzoom'],
                         ['jdaviz:boxzoom', 'jdaviz:xrangezoom', 'jdaviz:yrangezoom'],
                         ['jdaviz:panzoom', 'jdaviz:panzoom_x', 'jdaviz:panzoom_y'],
                     ]
         self._initialize_toolbar()
 
+        plugin.session.hub.broadcast(PluginPlotAddedMessage(sender=self))
+        plugin.session.hub.broadcast(PluginPlotModifiedMessage(sender=self))
+
     def _initialize_toolbar(self, default_tool_priority=[]):
         self.toolbar = NestedJupyterToolbar(self.viewer, self.tools_nested, default_tool_priority)
 
     @property
+    def user_api(self):
+        return UserApiWrapper(self, ('set_limits'))
+
+    @property
     def app(self):
         return self._app
 
     @property
     def layers(self):
         return {layer.layer.label: layer for layer in self.viewer.layers}
 
@@ -3476,14 +4521,16 @@
                 raise ValueError("histogram requires data entries with length > 1")
 
     def _remove_data(self, label):
         dc_entry = self.app.data_collection[label]
         self.viewer.remove_data(dc_entry)
         self.app.data_collection.remove(dc_entry)
 
+        self._plugin.session.hub.broadcast(PluginPlotModifiedMessage(sender=self))
+
     def _update_data(self, label, reset_lims=False, **kwargs):
         self._check_valid_components(**kwargs)
         if label not in self.app.data_collection:
             self._add_data(label, **kwargs)
             return
         data = self.app.data_collection[label]
 
@@ -3508,14 +4555,16 @@
                 style_state = {}
             self._remove_data(label)
             self._add_data(label, **kwargs)
             self.update_style(label, **style_state)
         if reset_lims:
             self.viewer.state.reset_limits()
 
+        self._plugin.session.hub.broadcast(PluginPlotModifiedMessage(sender=self))
+
     def update_style(self, label, **kwargs):
         kwargs.setdefault('visible', True)
         if label not in self.layers.keys():
             if not kwargs['visible']:
                 # then we were only trying to hide anyways
                 # (note: this ignores any other passed styles)
                 return
@@ -3535,14 +4584,16 @@
         lyr = self.layers[label]
         with delay_callback(lyr.state, *list(kwargs.keys())):
             for k, v in kwargs.items():
                 if k == 'layer' or k.endswith('_att'):
                     continue
                 setattr(lyr.state, k, v)
 
+        self._plugin.session.hub.broadcast(PluginPlotModifiedMessage(sender=self))
+
     def _add_data(self, label, **kwargs):
         self._check_valid_components(**kwargs)
         data = Data(label=label, **kwargs)
         dc = self.app.data_collection
         dc.append(data)
         dc_entry = dc[label]
 
@@ -3550,23 +4601,27 @@
             # we can assume the same units/components since this only accepts x and y
             ref_data = dc[0]
             links = [LinkSame(dc_entry.components[i], ref_data.components[i])
                      for i in range(1, len(ref_data.components))]
             dc.add_link(links)
         self.viewer.add_data(dc_entry)
 
+        self._plugin.session.hub.broadcast(PluginPlotModifiedMessage(sender=self))
+
     def _refresh_marks(self):
         # ensure all marks are drawn
         # NOTE: this seems to only be necessary for histogram viewers and may be an upstream bug
         # if that is fixed upstream, we should test to see if we can safely remove this method
         # and all calls to it
         other_marks = list(self.marks.values())
         layer_marks = [m for m in self.figure.marks if m not in other_marks]
         self.figure.marks = layer_marks + other_marks
 
+        self._plugin.session.hub.broadcast(PluginPlotModifiedMessage(sender=self))
+
     @property
     def marks(self):
         return self._marks
 
     def clear_marks(self, *mark_labels):
         with self.hold_sync():
             for mark_label, mark in self.marks.items():
@@ -3575,14 +4630,16 @@
                         # NOTE: cannot completely empty samples
                         # may want to also set mark.visible=False manually if clearing
                         # (but this will still at least clear any internal arrays)
                         mark.samples = [0]
                     else:
                         mark.x, mark.y = [], []
 
+        self._plugin.session.hub.broadcast(PluginPlotModifiedMessage(sender=self))
+
     def clear_all_marks(self):
         self.clear_marks(*self.marks.keys())
 
     def _add_mark(self, cls, label, xnorm=False, ynorm=False, **kwargs):
         """
         Parameters
         ----------
@@ -3605,14 +4662,17 @@
             else:
                 scales[dim] = self.figure.axes[0].scale
         mark = cls(scales=scales,
                    labels=[label],
                    **kwargs)
         self.figure.marks = self.figure.marks + [mark]
         self._marks[label] = mark
+
+        self._plugin.session.hub.broadcast(PluginPlotModifiedMessage(sender=self))
+
         return mark
 
     def add_line(self, label, x=[], y=[], xnorm=False, ynorm=False, **kwargs):
         return self._add_mark(bqplot.Lines, label, x=x, y=y,
                               xnorm=xnorm, ynorm=ynorm,
                               colors=kwargs.pop('color', kwargs.pop('colors', 'gray')),
                               **kwargs)
```

### Comparing `jdaviz-3.8.2/jdaviz/core/tests/test_autoconfig.py` & `jdaviz-3.9.0/jdaviz/core/tests/test_autoconfig.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/core/tests/test_custom_traitlets.py` & `jdaviz-3.9.0/jdaviz/core/tests/test_custom_traitlets.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/core/tests/test_data_menu.py` & `jdaviz-3.9.0/jdaviz/core/tests/test_data_menu.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/core/tests/test_helpers.py` & `jdaviz-3.9.0/jdaviz/core/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/core/tests/test_region_translators.py` & `jdaviz-3.9.0/jdaviz/core/tests/test_region_translators.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/core/tests/test_template_mixin.py` & `jdaviz-3.9.0/jdaviz/core/tests/test_template_mixin.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     expected_max = spectrum1d.spectral_axis[spectrum1d.spectral_axis.value <= 7400][-1]
     np.testing.assert_allclose(expected_min.value, 6666.66666667, atol=1e-5)
     np.testing.assert_allclose(expected_max.value, 7333.33333333, atol=1e-5)
     assert p.spectral_subset.selected_min_max(spectrum1d) == (6500 * u.AA, 7400 * u.AA)
 
     # check selected subset mask available via API:
     expected_mask_with_spectral_subset = (
-        (spectrum1d.wavelength.to(u.AA).value < 6500) |
-        (spectrum1d.wavelength.to(u.AA).value > 7400)
+        (spectrum1d.wavelength.to_value(u.AA) < 6500) |
+        (spectrum1d.wavelength.to_value(u.AA) > 7400)
     )
     assert np.all(
         expected_mask_with_spectral_subset == p.spectral_subset.selected_subset_mask
     )
 
     assert p.spectral_subset.app == p.app
     assert p.spectral_subset.spectrum_viewer == sv
@@ -106,21 +106,21 @@
     app = cubeviz_helper.app
     app.add_data(spectrum1d_cube, 'test')
     app.add_data_to_viewer("spectrum-viewer", "test")
     app.add_data_to_viewer("flux-viewer", "test")
     fv = app.get_viewer("flux-viewer")
     sv = app.get_viewer("spectrum-viewer")
 
-    # export plot uses the mixin
-    p = app.get_tray_item_from_name('g-export-plot')
+    # export plugin uses the mixin
+    p = cubeviz_helper.plugins['Export']
     assert len(p.viewer.ids) == 3
     assert len(p.viewer.references) == 3
     assert len(p.viewer.labels) == 3
     assert p.viewer.selected_obj == fv
 
     # set by reference
-    p.viewer_selected = 'spectrum-viewer'
+    p.viewer = 'spectrum-viewer'
     assert p.viewer.selected_obj == sv
 
     # try setting based on id instead of reference
-    p.viewer_selected = p.viewer.ids[0]
-    assert p.viewer_selected == p.viewer.labels[0]
+    p.viewer = p.viewer.ids[0]
+    assert p.viewer.selected == p.viewer.labels[0]
```

### Comparing `jdaviz-3.8.2/jdaviz/core/tools.py` & `jdaviz-3.9.0/jdaviz/configs/cubeviz/plugins/slice/slice.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,471 +1,386 @@
-import os
+import threading
 import time
+import warnings
 
 import numpy as np
-from echo import delay_callback
-from glue.config import viewer_tool
-from glue.core import HubListener
-from glue.viewers.common.tool import Tool
-from glue_jupyter.bqplot.common.tools import (CheckableTool,
-                                              HomeTool, BqplotPanZoomMode,
-                                              BqplotPanZoomXMode, BqplotPanZoomYMode,
-                                              BqplotRectangleMode, BqplotCircleMode,
-                                              BqplotEllipseMode, BqplotCircularAnnulusMode,
-                                              BqplotXRangeMode, BqplotYRangeMode,
-                                              BqplotSelectionTool,
-                                              INTERACT_COLOR)
-from bqplot.interacts import BrushSelector, BrushIntervalSelector
-
-from jdaviz.core.events import LineIdentifyMessage, SpectralMarksChangedMessage
-from jdaviz.core.marks import SpectralLine
-
-__all__ = []
-
-ICON_DIR = os.path.normpath(os.path.join(os.path.dirname(__file__), '..', 'data', 'icons'))
-
-
-# Override icons for built-in tools from glue-jupyter
-BqplotRectangleMode.icon = os.path.join(ICON_DIR, 'select_xy.svg')
-BqplotCircleMode.icon = os.path.join(ICON_DIR, 'select_circle.svg')
-BqplotEllipseMode.icon = os.path.join(ICON_DIR, 'select_ellipse.svg')
-BqplotCircularAnnulusMode.icon = os.path.join(ICON_DIR, 'select_annulus.svg')
-BqplotXRangeMode.icon = os.path.join(ICON_DIR, 'select_x.svg')
-BqplotYRangeMode.icon = os.path.join(ICON_DIR, 'select_y.svg')
-
-
-class _BaseZoomHistory:
-    # Mixin for custom zoom tools to be able to save their previous zoom state
-    # which is then used by the PrevZoom tool
-    def save_prev_zoom(self):
-        self.viewer._prev_limits = (self.viewer.state.x_min, self.viewer.state.x_max,
-                                    self.viewer.state.y_min, self.viewer.state.y_max)
-
-
-class _MatchedZoomMixin:
-    match_axes = ('x', 'y')
-    disable_matched_zoom_in_other_viewer = False
-
-    def _is_matched_viewer(self, viewer):
-        return True
-
-    def _iter_matched_viewers(self, include_self=False):
-        for viewer in self.viewer.session.application.viewers:
-            if viewer is self.viewer and not include_self:
-                continue
-            elif self._is_matched_viewer(viewer):
-                yield viewer
-
-    def _map_limits(self, from_viewer, to_viewer, limits={}):
-        return limits
-
-    def _post_activate(self):
-        return
-
-    @property
-    def match_keys(self):
-        keys = []
-        for ax in self.match_axes:
-            keys += [f'{ax}_min', f'{ax}_max']
-        return keys
-
-    def activate(self):
-        if self.disable_matched_zoom_in_other_viewer:
-            # mapping limits are not guaranteed to roundtrip, so we need to disable
-            # any linked tool in the "other" viewer
-            for viewer in self._iter_matched_viewers(include_self=False):
-                if isinstance(viewer.toolbar.active_tool, _MatchedZoomMixin):
-                    viewer.toolbar.active_tool_id = None
-
-        super().activate()
-        for k in self.match_keys:
-            self.viewer.state.add_callback(k, self.on_limits_change)
-
-        self._post_activate()
-
-        # Trigger a sync so the initial limits match
-        self.on_limits_change()
-
-    def deactivate(self):
-        for k in self.match_keys:
-            self.viewer.state.remove_callback(k, self.on_limits_change)
-
-        super().deactivate()
-
-    def on_limits_change(self, *args):
-        # from_lims: limits in the viewer belonging to the tool
-        from_lims = {k: getattr(self.viewer.state, k) for k in self.match_keys}
-
-        for viewer in self._iter_matched_viewers(include_self=False):
-            # orig_lims: limits in this "matched" viewer
-            # to_lims: proposed new limits for this "matched" viewer
-            orig_lims = {k: getattr(viewer.state, k) for k in self.match_keys}
-            to_lims = self._map_limits(self.viewer, viewer, from_lims)
-            with delay_callback(viewer.state, *self.match_keys):
-                for ax in self.match_axes:
-                    # to avoid recursion we'll only update the state if there is a change
-                    # outside a tolerance set by some fraction of the limits range
-                    if None in orig_lims.values():
-                        orig_range = np.inf
-                    else:
-                        orig_range = abs(orig_lims.get(f'{ax}_max') - orig_lims.get(f'{ax}_min'))
-                    to_range = abs(to_lims.get(f'{ax}_max') - to_lims.get(f'{ax}_min'))
-                    tol = 1e-6 * min(orig_range, to_range)
-
-                    for k in (f'{ax}_min', f'{ax}_max'):
-                        value = to_lims.get(k)
-                        orig_value = orig_lims.get(k)
-                        if not np.isnan(value) and (orig_value is None or
-                                                    abs(value-orig_lims.get(k, np.inf)) > tol):
-                            setattr(viewer.state, k, value)
-
-    def is_visible(self):
-        return len(self.viewer.jdaviz_app._viewer_store) > 1
-
-
-@viewer_tool
-class PrevZoom(Tool, _BaseZoomHistory):
-    icon = os.path.join(ICON_DIR, 'zoom_back.svg')
-    tool_id = 'jdaviz:prevzoom'
-    action_text = 'Previous zoom'
-    tool_tip = 'Back to previous zoom level'
-
-    def activate(self):
-        if self.viewer._prev_limits is None:
-            return
-        prev_limits = self.viewer._prev_limits
-        self.save_prev_zoom()
-        self.viewer.state.x_min, self.viewer.state.x_max, self.viewer.state.y_min, self.viewer.state.y_max = prev_limits  # noqa
-
-
-@viewer_tool
-class HomeZoom(HomeTool, _BaseZoomHistory):
-    icon = os.path.join(ICON_DIR, 'home.svg')
-    tool_id = 'jdaviz:homezoom'
-    action_text = 'Reset zoom'
-    tool_tip = 'Reset zoom to show all visible data'
-
-    def activate(self):
-        self.save_prev_zoom()
-        super().activate()
-
-
-@viewer_tool
-class PanZoom(BqplotPanZoomMode, _BaseZoomHistory):
-    icon = os.path.join(ICON_DIR, 'pan.svg')
-    tool_id = 'jdaviz:panzoom'
-
-    def activate(self):
-        self.save_prev_zoom()
-        super().activate()
-
-
-@viewer_tool
-class PanZoomX(BqplotPanZoomXMode, _BaseZoomHistory):
-    icon = os.path.join(ICON_DIR, 'pan_x.svg')
-    tool_id = 'jdaviz:panzoom_x'
-
-    def activate(self):
-        self.save_prev_zoom()
-        super().activate()
-
-
-@viewer_tool
-class PanZoomY(BqplotPanZoomYMode, _BaseZoomHistory):
-    icon = os.path.join(ICON_DIR, 'pan_y.svg')
-    tool_id = 'jdaviz:panzoom_y'
-
-    def activate(self):
-        self.save_prev_zoom()
-        super().activate()
+from astropy import units as u
+from astropy.units import UnitsWarning
+from astropy.utils.decorators import deprecated
+from traitlets import Bool, Int, Unicode, observe
+
+from jdaviz.configs.cubeviz.plugins.viewers import (WithSliceIndicator, WithSliceSelection,
+                                                    CubevizImageView)
+from jdaviz.configs.cubeviz.helper import _spectral_axis_names
+from jdaviz.core.custom_traitlets import FloatHandleEmpty
+from jdaviz.core.events import (AddDataMessage, SliceToolStateMessage,
+                                SliceSelectSliceMessage, SliceValueUpdatedMessage,
+                                NewViewerMessage, ViewerAddedMessage, ViewerRemovedMessage,
+                                GlobalDisplayUnitChanged)
+from jdaviz.core.registries import tray_registry
+from jdaviz.core.template_mixin import PluginTemplateMixin
+from jdaviz.core.user_api import PluginUserApi
+
+
+__all__ = ['Slice']
+
+
+@tray_registry('cubeviz-slice', label="Slice", viewer_requirements='spectrum')
+class Slice(PluginTemplateMixin):
+    """
+    See the :ref:`Slice Plugin Documentation <slice>` for more details.
+
+    Only the following attributes and methods are available through the
+    :ref:`public plugin API <plugin-apis>`:
+
+    * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.show`
+    * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.open_in_tray`
+    * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.close_in_tray`
+    * ``value``
+      Value (wavelength or frequency) of the current slice.  When setting this directly, it will
+      update automatically to the value corresponding to the nearest slice, if ``snap_to_slice`` is
+      enabled.
+    * ``show_indicator``
+      Whether to show indicator in spectral viewer when slice tool is inactive.
+    * ``show_value``
+      Whether to show slice value in label to right of indicator.
+    """
+    _cube_viewer_cls = CubevizImageView
+    _cube_viewer_default_label = 'flux-viewer'
+    cube_viewer_exists = Bool(True).tag(sync=True)
+
+    allow_disable_snapping = Bool(False).tag(sync=True)  # noqa internal use to show and allow disabling snap-to-slice
+
+    template_file = __file__, "slice.vue"
+    value = FloatHandleEmpty().tag(sync=True)
+    value_label = Unicode("Value").tag(sync=True)
+    value_unit = Unicode("").tag(sync=True)
+    value_editing = Bool(False).tag(sync=True)  # whether the value input is actively being edited
+
+    slider_throttle = Int(200).tag(sync=True)  # milliseconds
+
+    snap_to_slice = Bool(True).tag(sync=True)
+    show_indicator = Bool(True).tag(sync=True)
+    show_value = Bool(True).tag(sync=True)
 
+    is_playing = Bool(False).tag(sync=True)
+    play_interval = Int(200).tag(sync=True)  # milliseconds
 
-class _BaseSelectZoom(BqplotSelectionTool, _BaseZoomHistory):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.reset()
 
-    def _new_interact(self):
-        raise NotImplementedError(f"_new_interact not implemented by {self.__class__.__name__}")
+        self._indicator_initialized = False
+        self._player = None
 
-    def reset(self):
-        if hasattr(self, 'interact'):
-            self.interact.close()
-        self.interact = self._new_interact()
-        self.interact.observe(self.on_brushing, "brushing")
+        # Subscribe to requests from the helper to change the slice across all viewers
+        self.session.hub.subscribe(self, SliceSelectSliceMessage,
+                                   handler=self._on_select_slice_message)
+
+        # Listen for new viewers/data.
+        self.session.hub.subscribe(self, ViewerAddedMessage,
+                                   handler=self._on_viewer_added)
+        self.session.hub.subscribe(self, ViewerRemovedMessage,
+                                   handler=self._on_viewer_removed)
+        self.hub.subscribe(self, AddDataMessage,
+                           handler=self._on_add_data)
+
+        # connect any pre-existing viewers
+        for viewer in self.app._viewer_store.values():
+            self._connect_viewer(viewer)
+
+        # initialize if cube viewer exists
+        self._check_if_cube_viewer_exists()
+
+        # update internal value (wavelength/frequency) when x display unit is changed
+        # so that the current slice number is preserved
+        self.session.hub.subscribe(self, GlobalDisplayUnitChanged,
+                                   handler=self._on_global_display_unit_changed)
+        self._initialize_location()
+
+    def _initialize_location(self, *args):
+        # initialize value_unit (this has to wait until data is loaded to an existing
+        # slice_indicator_viewer, so we'll keep trying until it is set - after that, changes
+        # will be handled by a change to global display units)
+        if not self.value_unit:
+            for viewer in self.slice_indicator_viewers:
+                # ignore while x_display_unit is unset or still degrees (before data transpose)
+                # if we ever need the slice axis to be degrees, this will need to be loosened
+                if getattr(viewer.state, 'x_display_unit', None) not in (None, 'deg'):
+                    self.value_unit = viewer.state.x_display_unit
+                    break
 
-    def on_brushing(self, msg):
-        if self.interact.brushing:
-            # start drawing a box, don't need to do anything
+        if self._indicator_initialized:
             return
 
-        self.save_prev_zoom()
-
-        with delay_callback(self.viewer.state, 'x_min', 'x_max', 'y_min', 'y_max'):
-            # implement on_update_zoom to act on the applicable interact Selector
-            self.on_update_zoom()
-
-        # reset destroys the current interact and replaces with a new one to avoid having
-        # the draggable selection
-        self.reset()
-        # activate automatically activates the new interact so that another zoom is possible
-        # until deselecting the zoom tool
-        self.activate()
-
-
-@viewer_tool
-class BoxZoom(_BaseSelectZoom):
-    icon = os.path.join(ICON_DIR, 'zoom_box.svg')
-    tool_id = 'jdaviz:boxzoom'
-    action_text = 'Box zoom'
-    tool_tip = 'Zoom to a drawn rectangle'
-
-    def _new_interact(self):
-        return BrushSelector(x_scale=self.viewer.scale_x,
-                             y_scale=self.viewer.scale_y,
-                             color=INTERACT_COLOR)
-
-    def on_update_zoom(self):
-        if self.interact.selected_x is None or self.interact.selected_y is None:
-            # a valid box was not drawn, perhaps just a click with no drag!
-            # let's ignore and reset the tool
-            return
+        # set initial value (and snap to nearest point, if enabled)
+        # we'll loop over all slice indicator viewers and their layers
+        # and just use the first layer with data.  Once initialized, this logic will be
+        # skipped going forward to not change any user selection (so will default to the
+        # middle of the first found layer)
+        for viewer in self.slice_indicator_viewers:
+            if str(viewer.state.x_att) not in self.valid_slice_att_names:
+                # avoid setting value to degs, before x_att is changed to wavelength, for example
+                continue
+            slice_values = viewer.slice_values
+            if len(slice_values):
+                self.value = slice_values[int(len(slice_values)/2)]
+                self._indicator_initialized = True
+                return
 
-        new_interact_x = self.get_x_axis_with_aspect_ratio()
-        self.viewer.state.y_min, self.viewer.state.y_max = self.interact.selected_y
+    @property
+    def slice_axis(self):
+        # global display unit "axis" corresponding to the slice axis
+        return 'spectral'
 
-        # Change the x axis to make sure all y axis values from the box zoom are included
-        self.viewer.state.x_min, self.viewer.state.x_max = new_interact_x
+    @property
+    def valid_slice_att_names(self):
+        return _spectral_axis_names + ['Pixel Axis 2 [x]']
 
-    def get_x_axis_with_aspect_ratio(self):
-        new_interact_x = self.interact.selected_x
-        # If aspect is equal, then we need to preserve that aspect ratio
-        # even if the box zoom area does not.
-        if self.viewer.state.aspect == "equal":
-            fig_axes_ratio = ((self.viewer.state.x_max - self.viewer.state.x_min) /
-                              (self.viewer.state.y_max - self.viewer.state.y_min))
+    @property
+    def slice_selection_viewers(self):
+        return [v for v in self.app._viewer_store.values() if isinstance(v, WithSliceSelection)]
 
-            # The value at index of 1 will always be the larger of the two numbers
-            x_diff = self.interact.selected_x[1] - self.interact.selected_x[0]
-            y_diff = self.interact.selected_y[1] - self.interact.selected_y[0]
+    @property
+    def slice_indicator_viewers(self):
+        return [v for v in self.app._viewer_store.values() if isinstance(v, WithSliceIndicator)]
 
-            if x_diff < y_diff * fig_axes_ratio:
-                x_with_aspect = y_diff * fig_axes_ratio
-                x_centre = (self.interact.selected_x[0] + self.interact.selected_x[1]) / 2
-                new_interact_x = (x_centre - x_with_aspect / 2, x_centre + x_with_aspect / 2)
+    @property
+    @deprecated(since="3.9", alternative="value")
+    def wavelength(self):
+        return self.user_api.value
 
-        return new_interact_x
+    @property
+    @deprecated(since="3.9", alternative="value_unit")
+    def wavelength_unit(self):
+        return self.user_api.value_unit
 
+    @property
+    @deprecated(since="3.9", alternative="show_value")
+    def show_wavelength(self):
+        return self.user_api.show_value
 
-@viewer_tool
-class XRangeZoom(_BaseSelectZoom):
-    icon = os.path.join(ICON_DIR, 'zoom_xrange.svg')
-    tool_id = 'jdaviz:xrangezoom'
-    action_text = 'Horizontal zoom'
-    tool_tip = 'Zoom to a drawn horizontal region'
+    @property
+    @deprecated(since="3.9", alternative="value")
+    def slice(self):
+        # this assumes the first slice_selection_viewer (and layer)
+        return self.slice_selection_viewers[0].slice
+
+    @slice.setter
+    @deprecated(since="3.9", alternative="value")
+    def slice(self, slice):
+        # this assumes the first slice_selection_viewer (and layer)
+        value = self.slice_selection_viewers[0].slice_values[slice]
+        self.value = value
 
-    def _new_interact(self):
-        return BrushIntervalSelector(scale=self.viewer.scale_x,
-                                     color=INTERACT_COLOR)
+    @property
+    def user_api(self):
+        # NOTE: remove slice, wavelength, show_wavelength after deprecation period
+        expose = ['slice', 'wavelength', 'show_wavelength',
+                  'value',
+                  'show_indicator', 'show_value']
+        if self.allow_disable_snapping:
+            expose += ['snap_to_slice']
+        return PluginUserApi(self, expose=expose)
+
+    def _check_if_cube_viewer_exists(self, *args):
+        for viewer in self.app._viewer_store.values():
+            if isinstance(viewer, self._cube_viewer_cls):
+                self.cube_viewer_exists = True
+                return
+        self.cube_viewer_exists = False
+
+    def vue_create_cube_viewer(self, *args):
+        self.app._on_new_viewer(NewViewerMessage(self._cube_viewer_cls, data=None, sender=self.app),
+                                vid=self._cube_viewer_default_label,
+                                name=self._cube_viewer_default_label)
+
+        dc = self.app.data_collection
+        for data in dc:
+            if data.ndim == 3:
+                # only load the first cube-like data
+                self.app.set_data_visibility(self._cube_viewer_default_label, data.label, True)
+                break
+
+    def _connect_viewer(self, viewer):
+        if isinstance(viewer, WithSliceIndicator):
+            # NOTE: on first call, this will initialize the indicator itself
+            viewer._set_slice_indicator_value(self.value)
+        # in the case where x_att is changed after the viewer is added or data is loaded, we
+        # may still need to initialize the location to a valid value (with a valid x_att)
+        viewer.state.add_callback('x_att', self._initialize_location)
+
+    def _on_viewer_added(self, msg):
+        viewer = self.app.get_viewer(msg.viewer_id)
+        self._connect_viewer(viewer)
+        self._check_if_cube_viewer_exists()
+
+    def _on_viewer_removed(self, msg):
+        self._check_if_cube_viewer_exists()
+
+    def _on_add_data(self, msg):
+        self._initialize_location()
+        if isinstance(msg.viewer, WithSliceSelection):
+            # instead of just setting viewer.slice_value, we'll make sure the "snapping" logic
+            # is updated (if enabled)
+            self._on_value_updated({'new': self.value})
+
+    def _on_select_slice_message(self, msg):
+        with warnings.catch_warnings():
+            warnings.simplefilter('ignore', category=UnitsWarning)
+            self.value = msg.value
 
-    def on_update_zoom(self):
-        if self.interact.selected is None:
-            # a valid region was not drawn, perhaps just a click with no drag!
-            # let's ignore and reset the tool
+    def _on_global_display_unit_changed(self, msg):
+        if msg.axis != self.slice_axis:
             return
-
-        self.viewer.state.x_min, self.viewer.state.x_max = self.interact.selected
-
-
-@viewer_tool
-class YRangeZoom(_BaseSelectZoom):
-    icon = os.path.join(ICON_DIR, 'zoom_yrange.svg')
-    tool_id = 'jdaviz:yrangezoom'
-    action_text = 'Vertical zoom'
-    tool_tip = 'Zoom to a drawn vertical region'
-
-    def _new_interact(self):
-        return BrushIntervalSelector(orientation='vertical',
-                                     scale=self.viewer.scale_y,
-                                     color=INTERACT_COLOR)
-
-    def on_update_zoom(self):
-        if self.interact.selected is None:
-            # a valid region was not drawn, perhaps just a click with no drag!
-            # let's ignore and reset the tool
+        if not self.value_unit:
+            self.value_unit = str(msg.unit)
             return
+        prev_unit = u.Unit(self.value_unit)
+        self.value_unit = str(msg.unit)
+        self.value = (self.value * prev_unit).to_value(msg.unit)
 
-        self.viewer.state.y_min, self.viewer.state.y_max = self.interact.selected
-
-
-@viewer_tool
-class SelectLine(CheckableTool, HubListener):
-    icon = os.path.join(ICON_DIR, 'line_select.svg')
-    tool_id = 'jdaviz:selectline'
-    action_text = 'Select/identify spectral line'
-    tool_tip = 'Select/identify spectral line'
+    @property
+    def valid_selection_values(self):
+        # all available slice values from cubes (unsorted)
+        viewers = self.slice_selection_viewers
+        if not len(viewers):
+            return np.array([])
+        return np.unique(np.concatenate([viewer.slice_values for viewer in viewers]))
 
-    def __init__(self, viewer, **kwargs):
-        super().__init__(viewer, **kwargs)
-        self.line_marks = []
-        self.line_names = []
+    @property
+    def valid_selection_values_sorted(self):
+        # all available slice values from cubes (sorted)
+        return np.sort(self.valid_selection_values)
 
-        self.viewer.session.hub.subscribe(self, SpectralMarksChangedMessage,
-                                          handler=self._on_plotted_lines_changed)
+    @property
+    def valid_indicator_values(self):
+        # all x-values in indicator viewers (unsorted)
+        viewers = self.slice_indicator_viewers
+        if not len(viewers):
+            return np.array([])
+        return np.unique(np.concatenate([viewer.slice_values for viewer in viewers]))
 
-    def activate(self):
-        self.viewer.add_event_callback(self.on_mouse_event,
-                                       events=['click'])
+    @property
+    def valid_indicator_values_sorted(self):
+        return np.sort(self.valid_indicator_values)
 
-    def deactivate(self):
-        self.viewer.remove_event_callback(self.on_mouse_event)
+    @property
+    def valid_values(self):
+        return self.valid_selection_values if self.cube_viewer_exists else self.valid_indicator_values  # noqa
 
-    def _on_plotted_lines_changed(self, msg):
-        self.line_marks = msg.marks
-        self.line_names = msg.names_rest
+    @property
+    def valid_values_sorted(self):
+        return self.valid_selection_values_sorted if self.cube_viewer_exists else self.valid_indicator_values_sorted  # noqa
 
-    def on_mouse_event(self, data):
-        # yes this would be avoid a list-comprehension by putting in
-        # _on_plotted_lines_changed, but by leaving it here, we let
-        # the marks worry about unit conversions
-        lines_x = np.array([mark.obs_value for mark in self.line_marks])
-        if not len(lines_x):
+    @observe('value')
+    def _on_value_updated(self, event):
+        # convert to float (JS handles stripping any invalid characters)
+        if not isinstance(event.get('new'), float):
+            try:
+                self.value = float(event.get('new'))
+            except ValueError:
+                return
             return
-        ind = np.argmin(abs(lines_x - data['domain']['x']))
-        # find line closest to mouse position and transmit event
-        msg = LineIdentifyMessage(self.line_names[ind], sender=self)
-        self.viewer.session.hub.broadcast(msg)
-
-    def is_visible(self):
-        return len([m for m in self.viewer.figure.marks if isinstance(m, SpectralLine)]) > 0
 
+        if self.snap_to_slice and not self.value_editing:
+            valid_values = self.valid_selection_values
+            if len(valid_values):
+                closest_ind = np.argmin(abs(valid_values - self.value))
+                closest_value = valid_values[closest_ind]
+                if self.value != closest_value:
+                    # cast to float in case closest_value is an integer (which would otherwise
+                    # raise an error with setting to the float traitlet)
+                    self.value = float(closest_value)
+                    # will trigger another call to this method
+                    return
+
+        for viewer in self.slice_indicator_viewers:
+            viewer._set_slice_indicator_value(self.value)
+        for viewer in self.slice_selection_viewers:
+            viewer.slice_value = self.value
+
+        self.hub.broadcast(SliceValueUpdatedMessage(value=self.value,
+                                                    value_unit=self.value_unit,
+                                                    sender=self))
+
+    @observe('snap_to_slice', 'value_editing')
+    def _on_snap_to_slice_changed(self, event):
+        if self.snap_to_slice and not self.value_editing:
+            self._on_value_updated({'new': self.value})
+
+    @observe('show_indicator', 'show_value')
+    def _on_setting_changed(self, event):
+        msg = SliceToolStateMessage({event['name']: event['new']}, viewer=None, sender=self)
+        self.session.hub.broadcast(msg)
 
-@viewer_tool
-class StretchBounds(CheckableTool):
-    icon = os.path.join(ICON_DIR, 'stretch_bounds.svg')
-    tool_id = 'jdaviz:stretch_bounds'
-    action_text = 'Set Stretch VMin and VMax'
-    tool_tip = 'Set closest stretch bound (VMin/VMax) with click or click+drag'
-
-    def __init__(self, viewer, **kwargs):
-        self._time_last = 0
-        super().__init__(viewer, **kwargs)
-
-    def activate(self):
-        self.viewer.add_event_callback(self.on_mouse_event,
-                                       events=['dragmove', 'click'])
-        for mark in self.viewer.figure.marks:
-            if np.any([x in mark.labels for x in ('vmin', 'vmax')]):
-                mark.colors = ["#c75d2c"]
-
-    def deactivate(self):
-        self.viewer.remove_event_callback(self.on_mouse_event)
-        for mark in self.viewer.figure.marks:
-            if np.any([x in mark.labels for x in ('vmin', 'vmax')]):
-                mark.colors = ["#007BA1"]
-
-    def on_mouse_event(self, data):
-        if (time.time() - self._time_last) <= 0.05:
-            # throttle to 200ms
+    def vue_goto_first(self, *args):
+        if self.is_playing:
             return
+        self.value = np.nanmin(self.valid_values)
 
-        event_x = data['domain']['x']
-        current_bounds = [self.viewer._plugin.stretch_vmin_value,
-                          self.viewer._plugin.stretch_vmax_value,]
-        att_names = ["stretch_vmin_value", "stretch_vmax_value"]
-        closest_bound_ind = np.argmin([abs(current_bounds[0] - event_x),
-                                       abs(current_bounds[1] - event_x)])
-
-        setattr(self.viewer._plugin, att_names[closest_bound_ind], event_x)
-
-        self._time_last = time.time()
-
-
-class _BaseSidebarShortcut(Tool):
-    plugin_name = None  # define in subclass
-    viewer_attr = 'viewer'
-
-    def activate(self):
-        plugin = self.viewer.jdaviz_app.get_tray_item_from_name(self.plugin_name)
-        plugin.open_in_tray()
-        viewer_id = self.viewer.reference_id
-        viewer_select = getattr(plugin, self.viewer_attr)
-        if viewer_select.multiselect:
-            viewer_id = [viewer_id]
-        setattr(viewer_select, 'selected', viewer_id)
-
-
-@viewer_tool
-class SidebarShortcutPlotOptions(_BaseSidebarShortcut):
-    plugin_name = 'g-plot-options'
-
-    icon = os.path.join(ICON_DIR, 'tune.svg')
-    tool_id = 'jdaviz:sidebar_plot'
-    action_text = 'Plot Options'
-    tool_tip = 'Open plot options plugin in sidebar'
-
-
-@viewer_tool
-class SidebarShortcutExportPlot(_BaseSidebarShortcut):
-    plugin_name = 'g-export-plot'
-
-    icon = os.path.join(ICON_DIR, 'image.svg')
-    tool_id = 'jdaviz:sidebar_export'
-    action_text = 'Export plot'
-    tool_tip = 'Open export plot plugin in sidebar'
-
-
-@viewer_tool
-class SidebarShortcutCompass(_BaseSidebarShortcut):
-    plugin_name = 'imviz-compass'
-
-    icon = os.path.join(ICON_DIR, 'compass.svg')
-    tool_id = 'jdaviz:sidebar_compass'
-    action_text = 'Compass'
-    tool_tip = 'Open compass plugin in sidebar'
-
-
-@viewer_tool
-class SinglePixelRegion(CheckableTool):
-
-    icon = os.path.join(ICON_DIR, 'select_single_pixel.svg')
-    tool_id = 'jdaviz:singlepixelregion'
-    action_text = 'Create single-pixel spatial region'
-    tool_tip = 'Define a single-pixel spatial region of interest'
-
-    def activate(self):
-        # This is copied from glue-jupyter's BqplotSelectionTool (but we don't inherit
-        # from that because that in turn inherits from InteractCheckableTool which requires
-        # setting self.interact)
-        if self.viewer.session.application.get_setting('new_subset_on_selection_tool_change'):
-            self.viewer.session.edit_subset_mode.edit_subset = None
-
-        self.viewer.add_event_callback(self.on_mouse_event, events=['click'])
-
-    def deactivate(self):
-        self.viewer.remove_event_callback(self.on_mouse_event)
+    def vue_goto_last(self, *args):
+        if self.is_playing:
+            return
+        self.value = np.nanmax(self.valid_values)
 
-    def on_mouse_event(self, data):
-        # Extract data coordinates - these are pixels in the reference image.
-        # NOTE: We always use the reference image pixel coordinates because
-        # Subset is defined w.r.t. reference image.
-        x = data['domain']['x']
-        y = data['domain']['y']
+    def vue_play_prev(self, *args):
+        if self.is_playing:
+            return
+        valid_values = self.valid_values_sorted
+        if not len(valid_values):
+            return
+        current_ind = np.argmin(abs(valid_values - self.value))
+        if current_ind == 0:
+            # wrap
+            self.value = valid_values[len(valid_values) - 1]
+        else:
+            self.value = valid_values[current_ind - 1]
 
-        if data['altKey'] is True:
-            reg = self.get_subset(x, y, as_roi=False)
-            self.viewer.jdaviz_helper.load_regions(reg)
+    def vue_play_next(self, *args):
+        if self.is_playing:
+            return
+        valid_values = self.valid_values_sorted
+        if not len(valid_values):
+            return
+        current_ind = np.argmin(abs(valid_values - self.value))
+        if len(valid_values) <= current_ind + 1:
+            # wrap
+            self.value = valid_values[0]
         else:
-            roi = self.get_subset(x, y, as_roi=True)
-            self.viewer.apply_roi(roi)
+            self.value = valid_values[current_ind + 1]
+
+    def _player_worker(self):
+        ts = float(self.play_interval) * 1e-3  # ms to s
+        valid_values = self.valid_values_sorted
+        if not len(valid_values):
+            self.is_playing = False
+            return
+        while self.is_playing:
+            # recompute current_ind in case user has moved slider
+            # could optimize this by only recomputing after a select slice message
+            # (will only make a difference if argmin becomes approaches play_interval)
+            current_ind = np.argmin(abs(valid_values - self.value))
+            if len(valid_values) <= current_ind + 1:
+                # wrap
+                self.value = valid_values[0]
+            else:
+                self.value = valid_values[current_ind + 1]
+            time.sleep(ts)
+
+    def vue_play_start_stop(self, *args):
+        if self.is_playing:  # Stop
+            if self._player:
+                if self._player.is_alive():
+                    self._player.join(timeout=0)
+                self._player = None
+            self.is_playing = False
+            return
 
-    def get_subset(self, x, y, as_roi=False):
-        from regions import RectanglePixelRegion, PixCoord
-        x, y = np.rint([x, y])  # Center on nearest pixel
-        reg = RectanglePixelRegion(center=PixCoord(x=x, y=y), width=1, height=1)
-
-        if as_roi:
-            from jdaviz.core.region_translators import regions2roi
-            roi = regions2roi(reg)
-            return roi
+        if len(self.slice_indicator_viewers) == 0 and len(self.slice_selection_viewers) == 0:
+            return
+        if not len(self.valid_values_sorted):
+            return
 
-        return reg
+        # Start
+        self.is_playing = True
+        self._player = threading.Thread(target=self._player_worker)
+        self._player.start()
```

### Comparing `jdaviz-3.8.2/jdaviz/core/validunits.py` & `jdaviz-3.9.0/jdaviz/core/validunits.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/checktoradial.svg` & `jdaviz-3.9.0/jdaviz/data/icons/checktoradial.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/compass.svg` & `jdaviz-3.9.0/jdaviz/data/icons/compass.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/cubeviz_icon.svg` & `jdaviz-3.9.0/jdaviz/data/icons/cubeviz_icon.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/home_match.svg` & `jdaviz-3.9.0/jdaviz/data/icons/home_match.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/imviz_icon.svg` & `jdaviz-3.9.0/jdaviz/data/icons/imviz_icon.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/line_select.svg` & `jdaviz-3.9.0/jdaviz/data/icons/line_select.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/line_select_disabled.svg` & `jdaviz-3.9.0/jdaviz/data/icons/line_select_disabled.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/mosviz_icon.svg` & `jdaviz-3.9.0/jdaviz/data/icons/mosviz_icon.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/pan.svg` & `jdaviz-3.9.0/jdaviz/data/icons/pan.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/pan2.svg` & `jdaviz-3.9.0/jdaviz/data/icons/pan2.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/pan_x_match.svg` & `jdaviz-3.9.0/jdaviz/data/icons/pan_x_match.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/pan_y_match.svg` & `jdaviz-3.9.0/jdaviz/data/icons/pan_y_match.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/panzoom_match.svg` & `jdaviz-3.9.0/jdaviz/data/icons/panzoom_match.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/pixelspectra.svg` & `jdaviz-3.9.0/jdaviz/data/icons/pixelspectra.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/radialtocheck.svg` & `jdaviz-3.9.0/jdaviz/data/icons/radialtocheck.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/select_annulus.svg` & `jdaviz-3.9.0/jdaviz/data/icons/select_annulus.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/select_circle.svg` & `jdaviz-3.9.0/jdaviz/data/icons/select_circle.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/select_ellipse.svg` & `jdaviz-3.9.0/jdaviz/data/icons/select_ellipse.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/select_lasso.svg` & `jdaviz-3.9.0/jdaviz/data/icons/select_lasso.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/select_single_pixel.svg` & `jdaviz-3.9.0/jdaviz/data/icons/select_single_pixel.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/select_xy.svg` & `jdaviz-3.9.0/jdaviz/data/icons/select_xy.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/slice.svg` & `jdaviz-3.9.0/jdaviz/data/icons/slice.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/spectral_range.svg` & `jdaviz-3.9.0/jdaviz/data/icons/spectral_range.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/specviz2d_icon.svg` & `jdaviz-3.9.0/jdaviz/data/icons/specviz2d_icon.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/specviz_icon.svg` & `jdaviz-3.9.0/jdaviz/data/icons/specviz_icon.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/stretch_bounds.svg` & `jdaviz-3.9.0/jdaviz/data/icons/stretch_bounds.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/zoom_box.svg` & `jdaviz-3.9.0/jdaviz/data/icons/zoom_box.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/zoom_box_match.svg` & `jdaviz-3.9.0/jdaviz/data/icons/zoom_box_match.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/zoom_xrange.svg` & `jdaviz-3.9.0/jdaviz/data/icons/zoom_xrange.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/zoom_xrange_match.svg` & `jdaviz-3.9.0/jdaviz/data/icons/zoom_xrange_match.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/zoom_yrange.svg` & `jdaviz-3.9.0/jdaviz/data/icons/zoom_yrange.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/icons/zoom_yrange_match.svg` & `jdaviz-3.9.0/jdaviz/data/icons/zoom_yrange_match.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/linelists/Atomic-ISO.csv` & `jdaviz-3.9.0/jdaviz/data/linelists/Atomic-ISO.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/linelists/Atomic-Ionic.csv` & `jdaviz-3.9.0/jdaviz/data/linelists/Atomic-Ionic.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/linelists/Atomic-Ionic_FineStructure.csv` & `jdaviz-3.9.0/jdaviz/data/linelists/Atomic-Ionic_FineStructure.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/linelists/CO.csv` & `jdaviz-3.9.0/jdaviz/data/linelists/CO.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/linelists/Common_Galactic_2000A-11000A.csv` & `jdaviz-3.9.0/jdaviz/data/linelists/Common_Galactic_2000A-11000A.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/linelists/Common_Galactic_700A-2000A.csv` & `jdaviz-3.9.0/jdaviz/data/linelists/Common_Galactic_700A-2000A.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/linelists/Common_nebular.csv` & `jdaviz-3.9.0/jdaviz/data/linelists/Common_nebular.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/linelists/Common_stellar.csv` & `jdaviz-3.9.0/jdaviz/data/linelists/Common_stellar.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/linelists/DEV_NOTES.txt` & `jdaviz-3.9.0/jdaviz/data/linelists/DEV_NOTES.txt`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/linelists/H-He.csv` & `jdaviz-3.9.0/jdaviz/data/linelists/H-He.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/linelists/H-Paschen-Brackett.csv` & `jdaviz-3.9.0/jdaviz/data/linelists/H-Paschen-Brackett.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/linelists/H2-ISO.csv` & `jdaviz-3.9.0/jdaviz/data/linelists/H2-ISO.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/linelists/H2-alt.csv` & `jdaviz-3.9.0/jdaviz/data/linelists/H2-alt.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/linelists/H2.csv` & `jdaviz-3.9.0/jdaviz/data/linelists/H2.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/linelists/HeI-HeII.csv` & `jdaviz-3.9.0/jdaviz/data/linelists/HeI-HeII.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/linelists/JWST_line_list_original.txt` & `jdaviz-3.9.0/jdaviz/data/linelists/JWST_line_list_original.txt`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/linelists/PAH.csv` & `jdaviz-3.9.0/jdaviz/data/linelists/PAH.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/linelists/SDSS-IV.csv` & `jdaviz-3.9.0/jdaviz/data/linelists/SDSS-IV.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/linelists/SDSS.csv` & `jdaviz-3.9.0/jdaviz/data/linelists/SDSS.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/linelists/UV_linelist_vacuum.csv` & `jdaviz-3.9.0/jdaviz/data/linelists/UV_linelist_vacuum.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/data/linelists/linelist_metadata.json` & `jdaviz-3.9.0/jdaviz/data/linelists/linelist_metadata.json`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/jdaviz_cli.ipynb` & `jdaviz-3.9.0/jdaviz/jdaviz_cli.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/jdaviz_cli_launcher.ipynb` & `jdaviz-3.9.0/jdaviz/jdaviz_cli_launcher.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/models/physical_models.py` & `jdaviz-3.9.0/jdaviz/models/physical_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         bb = BlackBody(temperature=5778*u.K)
         wav = np.arange(1000, 110000) * u.AA
         flux = bb(wav)
 
         with quantity_support():
             plt.figure()
             plt.semilogx(wav, flux)
-            plt.axvline(bb.nu_max.to(u.AA, equivalencies=u.spectral()).value, ls='--')
+            plt.axvline(bb.nu_max.to_value(u.AA, equivalencies=u.spectral()), ls='--')
             plt.show()
     """
 
     # We parametrize this model with a temperature and a scale.
     temperature = Parameter(default=5000.0, min=0, unit=u.K, description="Blackbody temperature")
     scale = Parameter(default=1.0, min=0, description="Scale factor")
```

### Comparing `jdaviz-3.8.2/jdaviz/tests/coveragerc` & `jdaviz-3.9.0/jdaviz/tests/coveragerc`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/tests/test_app.py` & `jdaviz-3.9.0/jdaviz/tests/test_app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 
+import numpy as np
 from jdaviz import Application, Specviz
 from jdaviz.configs.default.plugins.gaussian_smooth.gaussian_smooth import GaussianSmooth
 
 
 # This applies to all viz but testing with Imviz should be enough.
 def test_viewer_calling_app(imviz_helper):
     viewer = imviz_helper.default_viewer._obj
@@ -32,15 +33,15 @@
                        'g-plot-options',
                        'g-subset-plugin',
                        'g-gaussian-smooth',
                        'g-model-fitting',
                        'g-unit-conversion',
                        'g-line-list',
                        'specviz-line-analysis',
-                       'g-export-plot'],
+                       'export'],
               'viewer_area': [{'container': 'col',
                                'children': [{'container': 'row',
                                              'viewers': [{'name': 'H',
                                                           'plot': 'specviz-profile-viewer',
                                                           'reference': 'h'},
                                                          {'name': 'K',
                                                           'plot': 'specviz-profile-viewer',
@@ -166,7 +167,28 @@
         )
 
     with pytest.raises(ValueError, match="does not exist"):
         imviz_helper.app._update_viewer_reference_name(
             old_reference='non-existent',
             new_reference='this-is-forbidden'
         )
+
+
+def test_data_associations(imviz_helper):
+    shape = (10, 10)
+
+    data_parent = np.ones(shape, dtype=float)
+    data_child = np.zeros(shape, dtype=int)
+
+    imviz_helper.load_data(data_parent, data_label='parent_data')
+    imviz_helper.load_data(data_child, data_label='child_data', parent='parent_data')
+
+    assert imviz_helper.app._get_assoc_data_children('parent_data') == ['child_data']
+    assert imviz_helper.app._get_assoc_data_parent('child_data') == 'parent_data'
+
+    with pytest.raises(NotImplementedError):
+        # we don't (yet) allow children of children:
+        imviz_helper.load_data(data_child, data_label='grandchild_data', parent='child_data')
+
+    with pytest.raises(ValueError):
+        # ensure the parent actually exists:
+        imviz_helper.load_data(data_child, data_label='child_data', parent='absent parent')
```

### Comparing `jdaviz-3.8.2/jdaviz/tests/test_data_formats.py` & `jdaviz-3.9.0/jdaviz/tests/test_data_formats.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/tests/test_metadata.py` & `jdaviz-3.9.0/jdaviz/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/tests/test_plugin_is_active.py` & `jdaviz-3.9.0/jdaviz/tests/test_plugin_is_active.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/tests/test_subsets.py` & `jdaviz-3.9.0/jdaviz/tests/test_subsets.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,18 +39,18 @@
     assert_allclose(reg.height, 6.6)
     assert_allclose(reg.angle.value, 0)
 
     assert subset_plugin.subset_selected == "Subset 1"
     assert subset_plugin.subset_types == ["EllipticalROI"]
     assert subset_plugin.is_centerable
     for key in ("orig", "value"):
-        assert subset_plugin._get_value_from_subset_definition(0, "X Center", key) == 1
-        assert subset_plugin._get_value_from_subset_definition(0, "Y Center", key) == 3.5
-        assert subset_plugin._get_value_from_subset_definition(0, "X Radius", key) == 1.2
-        assert subset_plugin._get_value_from_subset_definition(0, "Y Radius", key) == 3.3
+        assert subset_plugin._get_value_from_subset_definition(0, "X Center (pixels)", key) == 1
+        assert subset_plugin._get_value_from_subset_definition(0, "Y Center (pixels)", key) == 3.5
+        assert subset_plugin._get_value_from_subset_definition(0, "X Radius (pixels)", key) == 1.2
+        assert subset_plugin._get_value_from_subset_definition(0, "Y Radius (pixels)", key) == 3.3
         assert subset_plugin._get_value_from_subset_definition(0, "Angle", key) == 0
 
     # Recenter GUI should not be exposed, but API call would raise exception.
     with pytest.raises(NotImplementedError, match='Cannot recenter'):
         subset_plugin.vue_recenter_subset()
 
 
@@ -78,34 +78,34 @@
     assert_allclose(reg.angle.value, 0)
 
     assert subset_plugin.subset_selected == "Subset 1"
     assert subset_plugin.subset_types == ["RectangularROI"]
     assert subset_plugin.is_centerable
     assert subset_plugin.get_center() == (2.25, 1.55)
     for key in ("orig", "value"):
-        assert subset_plugin._get_value_from_subset_definition(0, "Xmin", key) == 1
-        assert subset_plugin._get_value_from_subset_definition(0, "Xmax", key) == 3.5
-        assert subset_plugin._get_value_from_subset_definition(0, "Ymin", key) == -0.2
-        assert subset_plugin._get_value_from_subset_definition(0, "Ymax", key) == 3.3
+        assert subset_plugin._get_value_from_subset_definition(0, "Xmin (pixels)", key) == 1
+        assert subset_plugin._get_value_from_subset_definition(0, "Xmax (pixels)", key) == 3.5
+        assert subset_plugin._get_value_from_subset_definition(0, "Ymin (pixels)", key) == -0.2
+        assert subset_plugin._get_value_from_subset_definition(0, "Ymax (pixels)", key) == 3.3
         assert subset_plugin._get_value_from_subset_definition(0, "Angle", key) == 0
 
     # Mimic user changing something in Subset Tool GUI.
-    subset_plugin._set_value_in_subset_definition(0, "Xmin", "value", 2)
-    subset_plugin._set_value_in_subset_definition(0, "Ymin", "value", 0)
+    subset_plugin._set_value_in_subset_definition(0, "Xmin (pixels)", "value", 2)
+    subset_plugin._set_value_in_subset_definition(0, "Ymin (pixels)", "value", 0)
     subset_plugin._set_value_in_subset_definition(0, "Angle", "value", 45)  # ccw deg
     # "orig" is unchanged until user clicks Update button.
-    assert subset_plugin._get_value_from_subset_definition(0, "Xmin", "orig") == 1
-    assert subset_plugin._get_value_from_subset_definition(0, "Ymin", "orig") == -0.2
+    assert subset_plugin._get_value_from_subset_definition(0, "Xmin (pixels)", "orig") == 1
+    assert subset_plugin._get_value_from_subset_definition(0, "Ymin (pixels)", "orig") == -0.2
     assert subset_plugin._get_value_from_subset_definition(0, "Angle", "orig") == 0
     subset_plugin.vue_update_subset()
     for key in ("orig", "value"):
-        assert subset_plugin._get_value_from_subset_definition(0, "Xmin", key) == 2
-        assert subset_plugin._get_value_from_subset_definition(0, "Xmax", key) == 3.5
-        assert subset_plugin._get_value_from_subset_definition(0, "Ymin", key) == 0
-        assert subset_plugin._get_value_from_subset_definition(0, "Ymax", key) == 3.3
+        assert subset_plugin._get_value_from_subset_definition(0, "Xmin (pixels)", key) == 2
+        assert subset_plugin._get_value_from_subset_definition(0, "Xmax (pixels)", key) == 3.5
+        assert subset_plugin._get_value_from_subset_definition(0, "Ymin (pixels)", key) == 0
+        assert subset_plugin._get_value_from_subset_definition(0, "Ymax (pixels)", key) == 3.3
         assert subset_plugin._get_value_from_subset_definition(0, "Angle", key) == 45
 
     subsets = cubeviz_helper.app.get_subsets()
     reg = subsets.get('Subset 1')[0]['region']
 
     assert_allclose(reg.center.x, 2.75)
     assert_allclose(reg.center.y, 1.65)
@@ -128,33 +128,33 @@
     # We set the active tool here to trigger a reset of the Subset state to "Create New"
     flux_viewer.toolbar.active_tool = flux_viewer.toolbar.tools['bqplot:truecircle']
     cubeviz_helper.app.get_viewer('flux-viewer').apply_roi(CircularROI(xc=3, yc=4, radius=2.4))
     assert subset_plugin.subset_selected == "Subset 2"
     assert subset_plugin.subset_types == ["CircularROI"]
     assert subset_plugin.is_centerable
     for key in ("orig", "value"):
-        assert subset_plugin._get_value_from_subset_definition(0, "X Center", key) == 3
-        assert subset_plugin._get_value_from_subset_definition(0, "Y Center", key) == 4
-        assert subset_plugin._get_value_from_subset_definition(0, "Radius", key) == 2.4
+        assert subset_plugin._get_value_from_subset_definition(0, "X Center (pixels)", key) == 3
+        assert subset_plugin._get_value_from_subset_definition(0, "Y Center (pixels)", key) == 4
+        assert subset_plugin._get_value_from_subset_definition(0, "Radius (pixels)", key) == 2.4
 
     # Circular Annulus Subset
     flux_viewer = cubeviz_helper.app.get_viewer("flux-viewer")
     # We set the active tool here to trigger a reset of the Subset state to "Create New"
     flux_viewer.toolbar.active_tool = flux_viewer.toolbar.tools['bqplot:circannulus']
     cubeviz_helper.app.get_viewer('flux-viewer').apply_roi(CircularAnnulusROI(xc=5,
                                                                               yc=6,
                                                                               inner_radius=2,
                                                                               outer_radius=4))
     assert subset_plugin.subset_selected == "Subset 3"
     assert subset_plugin.subset_types == ["CircularAnnulusROI"]
     for key in ("orig", "value"):
-        assert subset_plugin._get_value_from_subset_definition(0, "X Center", key) == 5
-        assert subset_plugin._get_value_from_subset_definition(0, "Y Center", key) == 6
-        assert subset_plugin._get_value_from_subset_definition(0, "Inner radius", key) == 2
-        assert subset_plugin._get_value_from_subset_definition(0, "Outer radius", key) == 4
+        assert subset_plugin._get_value_from_subset_definition(0, "X Center (pixels)", key) == 5
+        assert subset_plugin._get_value_from_subset_definition(0, "Y Center (pixels)", key) == 6
+        assert subset_plugin._get_value_from_subset_definition(0, "Inner Radius (pixels)", key) == 2
+        assert subset_plugin._get_value_from_subset_definition(0, "Outer Radius (pixels)", key) == 4
 
 
 def test_region_from_subset_profile(cubeviz_helper, spectral_cube_wcs):
     data = Spectrum1D(flux=np.ones((128, 128, 256)) * u.nJy, wcs=spectral_cube_wcs)
     subset_plugin = cubeviz_helper.app.get_tray_item_from_name('g-subset-plugin')
 
     cubeviz_helper.load_data(data, data_label='Test 1D Flux')
@@ -482,15 +482,15 @@
 
     for layer in viewer.state.layers:
         if isinstance(layer.layer, GroupedSubset):
             assert get_subset_type(layer.layer.subset_state) == 'spatial'
 
 
 def test_composite_region_with_imviz(imviz_helper, image_2d_wcs):
-    arr = np.ones((10, 10))
+    arr = NDData(np.ones((10, 10)), wcs=image_2d_wcs)
 
     data_label = 'image-data'
     viewer = imviz_helper.default_viewer._obj
     imviz_helper.load_data(arr, data_label=data_label, show_in_viewer=True)
     viewer.apply_roi(CircularROI(xc=5, yc=5, radius=2))
     reg = imviz_helper.app.get_subsets("Subset 1")
     circle1 = CirclePixelRegion(center=PixCoord(x=5, y=5), radius=2)
@@ -536,45 +536,50 @@
         'data/gauss100_fits_wcs.fits', package='jdaviz.configs.imviz.tests'))
     # Different pixel scale
     imviz_helper.load_data(get_pkg_data_filename(
         'data/gauss100_fits_wcs_block_reduced.fits', package='jdaviz.configs.imviz.tests'))
 
     # Link them by WCS
     imviz_helper.link_data(link_type='wcs')
+    w = imviz_helper.app.data_collection[0].coords
 
     # This rectangle is over a real object in reference image but
     # only the last row in the second image if linked by pixel.
     imviz_helper.load_regions(
-        RectanglePixelRegion(center=PixCoord(x=229, y=152), width=17, height=7))
+        RectanglePixelRegion(center=PixCoord(x=229, y=152), width=17, height=7).to_sky(w))
 
     subset_plugin = imviz_helper.plugins["Subset Tools"]._obj
     subset_plugin.subset_selected = "Subset 1"
     subset_plugin.dataset_selected = "gauss100_fits_wcs_block_reduced[PRIMARY,1]"
 
     # Do it a few times to converge.
     for _ in range(5):
         subset_plugin.vue_recenter_subset()
 
     # If handled correctly, it won't change much.
     # But if not, it move down by 7 pix or so (229.05, 145.92) and fails the test.
-    assert_allclose(subset_plugin.get_center(), (229.067822, 152.371943))
+    xy = imviz_helper.default_viewer._obj._get_real_xy(
+        imviz_helper.app.data_collection[0], *subset_plugin.get_center())[:2]
+    assert_allclose(xy, (229.067822, 152.371943))
 
     # Now create a new subset that has a source in the corner and test
     # recentering with multiselect.
 
     imviz_helper.load_regions(
-        CirclePixelRegion(center=PixCoord(x=145, y=175), radius=17))
+        CirclePixelRegion(center=PixCoord(x=145, y=175), radius=17).to_sky(w))
     subset_plugin.multiselect = True
     subset_plugin.subset_selected = ["Subset 1", "Subset 2"]
 
     # Do it a few times to converge.
     for _ in range(5):
         subset_plugin.vue_recenter_subset()
 
-    assert_allclose(subset_plugin.get_center("Subset 2"), (145.593022, 172.515541))
+    xy = imviz_helper.default_viewer._obj._get_real_xy(
+        imviz_helper.app.data_collection[0], *subset_plugin.get_center("Subset 2"))[:2]
+    assert_allclose(xy, (145.593022, 172.515541))
 
     with pytest.raises(ValueError, match="Please include subset_name in"):
         subset_plugin.get_center()
     with pytest.raises(ValueError, match="Please include subset_name in"):
         subset_plugin.set_center((150, 200))
 
 
@@ -947,7 +952,42 @@
 
         data = NDData(np.ones((40, 40)) * u.nJy)
         imviz_helper.load_data(data)
 
         imviz_helper.app.get_viewer('imviz-0').apply_roi(CircularROI(25, 25, 10))
         subsets = imviz_helper.app.get_subsets(include_sky_region=True)
         assert subsets['Subset 1'][0]['sky_region'] is None
+
+    def test_subset_renaming(self, specviz_helper, spectrum1d):
+        specviz_helper.load_data(spectrum1d, 'myfile')
+        spectrum_viewer_name = specviz_helper._default_spectrum_viewer_reference_name
+        viewer = specviz_helper.app.get_viewer(spectrum_viewer_name)
+
+        viewer.apply_roi(XRangeROI(6200, 7200))
+        get_data_no_sub = specviz_helper.get_data('myfile')
+        get_data_1 = specviz_helper.get_data('myfile', spectral_subset='Subset 1')
+
+        get_data_1_mask = np.where(~get_data_1.mask)
+
+        # Retrieving data with no subset means mask is None
+        assert get_data_no_sub.mask is None
+        assert len(get_data_1_mask[0]) > 0
+
+        # rename subset to 'diffname'
+        subset_group = specviz_helper.app.data_collection.subset_groups
+        subset_group[0].label = 'diffname'
+        get_data_2 = specviz_helper.get_data('myfile', spectral_subset='diffname')
+
+        assert_quantity_allclose(get_data_1.flux, get_data_2.flux)
+        assert_quantity_allclose(get_data_1.spectral_axis, get_data_2.spectral_axis)
+        get_data_2_mask = np.where(~get_data_2.mask)
+        assert (get_data_1_mask[0] == get_data_2_mask[0]).all()
+
+        # when we officially implement subset renaming in jdaviz, we will want
+        # to be aware of the case of naming subsets after existing data
+        # and handle it appropriately
+        subset_group = specviz_helper.app.data_collection.subset_groups
+        subset_group[0].label = 'myfile'
+        get_data_3 = specviz_helper.get_data('myfile', spectral_subset='myfile')
+
+        get_data_3_mask = np.where(~get_data_3.mask)
+        assert (get_data_1_mask[0] == get_data_3_mask[0]).all()
```

### Comparing `jdaviz-3.8.2/jdaviz/tests/test_utils.py` & `jdaviz-3.9.0/jdaviz/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/tests/test_viewer_ids.py` & `jdaviz-3.9.0/jdaviz/tests/test_viewer_ids.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/jdaviz/utils.py` & `jdaviz-3.9.0/jdaviz/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import os
 import time
 import threading
 from collections import deque
-import numpy as np
 
+import numpy as np
 from astropy.io import fits
 from astropy.utils import minversion
-from ipyvue import watch
-from glue.core.exceptions import IncompatibleAttribute
+from astropy.wcs.wcsapi import BaseHighLevelWCS
 from glue.config import settings
+from glue.core import BaseData
+from glue.core.exceptions import IncompatibleAttribute
 from glue.core.subset import SubsetState, RangeSubsetState, RoiSubsetState
-
+from ipyvue import watch
 
 __all__ = ['SnackbarQueue', 'enable_hot_reloading', 'bqplot_clear_figure',
            'standardize_metadata', 'ColorCycler', 'alpha_index', 'get_subset_type']
 
 NUMPY_LT_2_0 = not minversion("numpy", "2.0.dev")
 
 # For Metadata Viewer plugin internal use only.
@@ -212,14 +213,46 @@
         # a-z
         return chr(97 + index)
     else:
         # aa-zz (26-701), then overflow strings like '{a'
         return chr(97 + index//26 - 1) + chr(97 + index % 26)
 
 
+def data_has_valid_wcs(data, ndim=None):
+    """Check if given glue Data has WCS that is compatible with APE 14."""
+    status = hasattr(data, 'coords') and isinstance(data.coords, BaseHighLevelWCS)
+    if ndim is not None:
+        status = status and data.coords.world_n_dim == ndim
+    return status
+
+
+def layer_is_table_data(layer):
+    return isinstance(layer, BaseData) and layer.ndim == 1
+
+
+_wcs_only_label = "_WCS_ONLY"
+
+
+def is_wcs_only(layer):
+    # exclude WCS-only layers from the layer choices:
+    if hasattr(layer, 'layer'):
+        state = layer.layer
+    elif hasattr(layer, 'data'):
+        state = layer.data
+    elif hasattr(layer, 'meta'):
+        state = layer
+    else:
+        raise NotImplementedError
+    return getattr(state, 'meta', {}).get(_wcs_only_label, False)
+
+
+def is_not_wcs_only(layer):
+    return not is_wcs_only(layer)
+
+
 def standardize_metadata(metadata):
     """Standardize given metadata so it can be viewed in
     Metadata Viewer plugin. The input can be plain
     dictionary or FITS header object. Output is just a plain
     dictionary.
     """
     if isinstance(metadata, fits.Header):
```

### Comparing `jdaviz-3.8.2/jdaviz.egg-info/PKG-INFO` & `jdaviz-3.9.0/jdaviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdaviz
-Version: 3.8.2
+Version: 3.9.0
 Summary: Astronomical data analysis development leveraging the Jupyter platform
 Author-email: JDADF Developers <help@stsci.edu>
 Project-URL: Homepage, https://jdaviz.readthedocs.io/en/latest/
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 Requires-Dist: packaging
```

### Comparing `jdaviz-3.8.2/jdaviz.egg-info/SOURCES.txt` & `jdaviz-3.9.0/jdaviz.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,21 @@
 conftest.py
 licenses
 pyproject.toml
 setup.py
 tox.ini
 .github/CODEOWNERS
 .github/PULL_REQUEST_TEMPLATE.md
+.github/dependabot.yml
 .github/labeler.yml
 .github/ISSUE_TEMPLATE/bug_report.yaml
 .github/ISSUE_TEMPLATE/config.yml
 .github/ISSUE_TEMPLATE/feature_request.yaml
 .github/workflows/changelog_check.yml
+.github/workflows/check_milestone.yml
 .github/workflows/ci_cron_weekly.yml
 .github/workflows/ci_workflows.yml
 .github/workflows/codeql-analysis.yml
 .github/workflows/open_actions.yml
 .github/workflows/predeps_workflows.yml
 .github/workflows/publish.yml
 .github/workflows/standalone.yml
@@ -34,40 +36,46 @@
 jdaviz/app.py
 jdaviz/app.vue
 jdaviz/cli.py
 jdaviz/conftest.py
 jdaviz/container.vue
 jdaviz/jdaviz_cli.ipynb
 jdaviz/jdaviz_cli_launcher.ipynb
+jdaviz/main_styles.vue
+jdaviz/style_registry.py
 jdaviz/utils.py
 jdaviz/version.py
 jdaviz.egg-info/PKG-INFO
 jdaviz.egg-info/SOURCES.txt
 jdaviz.egg-info/dependency_links.txt
 jdaviz.egg-info/entry_points.txt
 jdaviz.egg-info/not-zip-safe
 jdaviz.egg-info/requires.txt
 jdaviz.egg-info/top_level.txt
 jdaviz/components/__init__.py
 jdaviz/components/docs_link.vue
 jdaviz/components/external_link.vue
 jdaviz/components/glue_state_sync_wrapper.vue
 jdaviz/components/layer_viewer_icon.vue
+jdaviz/components/multiselect_toggle.vue
 jdaviz/components/number_uncertainty.vue
 jdaviz/components/play_pause_widget.vue
 jdaviz/components/plugin_action_button.vue
 jdaviz/components/plugin_add_results.vue
 jdaviz/components/plugin_auto_label.vue
 jdaviz/components/plugin_dataset_select.vue
 jdaviz/components/plugin_editable_select.vue
 jdaviz/components/plugin_file_import_select.vue
+jdaviz/components/plugin_inline_select.vue
+jdaviz/components/plugin_inline_select_item.vue
 jdaviz/components/plugin_layer_select.vue
 jdaviz/components/plugin_layer_select_tabs.vue
 jdaviz/components/plugin_plot.vue
 jdaviz/components/plugin_popout.vue
+jdaviz/components/plugin_previews_temp_disabled.vue
 jdaviz/components/plugin_section_header.vue
 jdaviz/components/plugin_subset_select.vue
 jdaviz/components/plugin_table.vue
 jdaviz/components/plugin_viewer_select.vue
 jdaviz/components/toolbar_nested.py
 jdaviz/components/toolbar_nested.vue
 jdaviz/components/tooltip.vue
@@ -95,14 +103,15 @@
 jdaviz/configs/cubeviz/plugins/slice/tests/test_slice.py
 jdaviz/configs/cubeviz/plugins/spectral_extraction/__init__.py
 jdaviz/configs/cubeviz/plugins/spectral_extraction/spectral_extraction.py
 jdaviz/configs/cubeviz/plugins/spectral_extraction/spectral_extraction.vue
 jdaviz/configs/cubeviz/plugins/spectral_extraction/tests/__init__.py
 jdaviz/configs/cubeviz/plugins/spectral_extraction/tests/test_spectral_extraction.py
 jdaviz/configs/cubeviz/plugins/tests/__init__.py
+jdaviz/configs/cubeviz/plugins/tests/test_cubeviz_aperphot.py
 jdaviz/configs/cubeviz/plugins/tests/test_cubeviz_helper.py
 jdaviz/configs/cubeviz/plugins/tests/test_data_retrieval.py
 jdaviz/configs/cubeviz/plugins/tests/test_data_selection.py
 jdaviz/configs/cubeviz/plugins/tests/test_export_plots.py
 jdaviz/configs/cubeviz/plugins/tests/test_parsers.py
 jdaviz/configs/cubeviz/plugins/tests/test_regions.py
 jdaviz/configs/cubeviz/plugins/tests/test_tools.py
@@ -112,21 +121,26 @@
 jdaviz/configs/default/plugins/__init__.py
 jdaviz/configs/default/plugins/viewers.py
 jdaviz/configs/default/plugins/collapse/__init__.py
 jdaviz/configs/default/plugins/collapse/collapse.py
 jdaviz/configs/default/plugins/collapse/collapse.vue
 jdaviz/configs/default/plugins/collapse/tests/__init__.py
 jdaviz/configs/default/plugins/collapse/tests/test_collapse.py
+jdaviz/configs/default/plugins/data_quality/__init__.py
+jdaviz/configs/default/plugins/data_quality/dq_utils.py
+jdaviz/configs/default/plugins/data_quality/tests/__init__.py
+jdaviz/configs/default/plugins/data_quality/tests/test_data_quality.py
 jdaviz/configs/default/plugins/data_tools/__init__.py
 jdaviz/configs/default/plugins/data_tools/data_tools.py
 jdaviz/configs/default/plugins/data_tools/data_tools.vue
 jdaviz/configs/default/plugins/data_tools/file_chooser.py
-jdaviz/configs/default/plugins/export_plot/__init__.py
-jdaviz/configs/default/plugins/export_plot/export_plot.py
-jdaviz/configs/default/plugins/export_plot/export_plot.vue
+jdaviz/configs/default/plugins/export/__init__.py
+jdaviz/configs/default/plugins/export/export.py
+jdaviz/configs/default/plugins/export/export.vue
+jdaviz/configs/default/plugins/export/tests/test_export.py
 jdaviz/configs/default/plugins/gaussian_smooth/__init__.py
 jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.py
 jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.vue
 jdaviz/configs/default/plugins/gaussian_smooth/tests/__init__.py
 jdaviz/configs/default/plugins/gaussian_smooth/tests/test_gaussian_smooth.py
 jdaviz/configs/default/plugins/line_lists/__init__.py
 jdaviz/configs/default/plugins/line_lists/line_list_mixin.py
@@ -157,14 +171,15 @@
 jdaviz/configs/default/plugins/plot_options/plot_options.py
 jdaviz/configs/default/plugins/plot_options/plot_options.vue
 jdaviz/configs/default/plugins/plot_options/tests/__init__.py
 jdaviz/configs/default/plugins/plot_options/tests/test_plot_options.py
 jdaviz/configs/default/plugins/subset_plugin/__init__.py
 jdaviz/configs/default/plugins/subset_plugin/subset_plugin.py
 jdaviz/configs/default/plugins/subset_plugin/subset_plugin.vue
+jdaviz/configs/default/plugins/subset_plugin/utils.py
 jdaviz/configs/default/plugins/subset_plugin/tests/__init__.py
 jdaviz/configs/default/plugins/subset_plugin/tests/test_subset_plugin.py
 jdaviz/configs/default/plugins/subset_tools/__init__.py
 jdaviz/configs/default/plugins/subset_tools/subset_tools.py
 jdaviz/configs/default/plugins/subset_tools/subset_tools.vue
 jdaviz/configs/default/plugins/viewer_creator/__init__.py
 jdaviz/configs/default/plugins/viewer_creator/viewer_creator.py
@@ -196,32 +211,32 @@
 jdaviz/configs/imviz/plugins/footprints/preset_regions.py
 jdaviz/configs/imviz/plugins/image_viewer_creator/__init__.py
 jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.py
 jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.vue
 jdaviz/configs/imviz/plugins/line_profile_xy/__init__.py
 jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.py
 jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.vue
-jdaviz/configs/imviz/plugins/links_control/__init__.py
-jdaviz/configs/imviz/plugins/links_control/links_control.py
-jdaviz/configs/imviz/plugins/links_control/links_control.vue
+jdaviz/configs/imviz/plugins/orientation/__init__.py
+jdaviz/configs/imviz/plugins/orientation/orientation.py
+jdaviz/configs/imviz/plugins/orientation/orientation.vue
 jdaviz/configs/imviz/plugins/rotate_canvas/__init__.py
 jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.py
 jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.vue
 jdaviz/configs/imviz/plugins/rotate_canvas/tests/__init__.py
 jdaviz/configs/imviz/plugins/rotate_canvas/tests/test_rotate_canvas.py
 jdaviz/configs/imviz/tests/__init__.py
 jdaviz/configs/imviz/tests/test_astrowidgets_api.py
 jdaviz/configs/imviz/tests/test_catalogs.py
 jdaviz/configs/imviz/tests/test_compass.py
 jdaviz/configs/imviz/tests/test_delete_data.py
 jdaviz/configs/imviz/tests/test_footprints.py
 jdaviz/configs/imviz/tests/test_helper.py
 jdaviz/configs/imviz/tests/test_line_profile_xy.py
 jdaviz/configs/imviz/tests/test_linking.py
-jdaviz/configs/imviz/tests/test_links_control.py
+jdaviz/configs/imviz/tests/test_orientation.py
 jdaviz/configs/imviz/tests/test_parser.py
 jdaviz/configs/imviz/tests/test_parser_asdf.py
 jdaviz/configs/imviz/tests/test_parser_roman.py
 jdaviz/configs/imviz/tests/test_regions.py
 jdaviz/configs/imviz/tests/test_simple_aper_phot.py
 jdaviz/configs/imviz/tests/test_subset_centroid.py
 jdaviz/configs/imviz/tests/test_tools.py
@@ -272,14 +287,15 @@
 jdaviz/configs/specviz/plugins/unit_conversion/__init__.py
 jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.py
 jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.vue
 jdaviz/configs/specviz/plugins/unit_conversion/tests/__init__.py
 jdaviz/configs/specviz/plugins/unit_conversion/tests/test_unit_conversion.py
 jdaviz/configs/specviz/tests/__init__.py
 jdaviz/configs/specviz/tests/test_helper.py
+jdaviz/configs/specviz/tests/test_viewers.py
 jdaviz/configs/specviz2d/__init__.py
 jdaviz/configs/specviz2d/helper.py
 jdaviz/configs/specviz2d/specviz2d.yaml
 jdaviz/configs/specviz2d/plugins/__init__.py
 jdaviz/configs/specviz2d/plugins/parsers.py
 jdaviz/configs/specviz2d/plugins/spectral_extraction/__init__.py
 jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.py
@@ -312,14 +328,16 @@
 jdaviz/core/tests/test_autoconfig.py
 jdaviz/core/tests/test_custom_traitlets.py
 jdaviz/core/tests/test_data_menu.py
 jdaviz/core/tests/test_helpers.py
 jdaviz/core/tests/test_region_translators.py
 jdaviz/core/tests/test_template_mixin.py
 jdaviz/core/tests/test_tools.py
+jdaviz/data/data_quality/jwst.csv
+jdaviz/data/data_quality/roman.csv
 jdaviz/data/icons/blink.svg
 jdaviz/data/icons/checktoradial.svg
 jdaviz/data/icons/compass.svg
 jdaviz/data/icons/contrast.svg
 jdaviz/data/icons/cubeviz_icon.svg
 jdaviz/data/icons/home.svg
 jdaviz/data/icons/home_match.svg
@@ -403,14 +421,15 @@
 notebooks/ImvizDitheredExample.ipynb
 notebooks/ImvizExample.ipynb
 notebooks/MosvizExample.ipynb
 notebooks/MosvizNIRISSExample.ipynb
 notebooks/Specviz2dExample.ipynb
 notebooks/SpecvizExample.ipynb
 notebooks/concepts/README.md
+notebooks/concepts/cubeviz_aperture_photometry.ipynb
 notebooks/concepts/cubeviz_contour_overlay.ipynb
 notebooks/concepts/cubeviz_data_interactions.ipynb
 notebooks/concepts/cubeviz_fitting.ipynb
 notebooks/concepts/cubeviz_ndarray_gif.ipynb
 notebooks/concepts/cubeviz_spectral_fitting.ipynb
 notebooks/concepts/cubeviz_spectral_spatial_interactions.ipynb
 notebooks/concepts/cubeviz_wfc3ir_ramp.ipynb
```

### Comparing `jdaviz-3.8.2/jdaviz.egg-info/requires.txt` & `jdaviz-3.9.0/jdaviz.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/licenses/GINGA_LICENSE.txt` & `jdaviz-3.9.0/licenses/GINGA_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/licenses/IMEXAM_LICENSE.txt` & `jdaviz-3.9.0/licenses/IMEXAM_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/licenses/IPYFILECHOOSER_LICENSE.rst` & `jdaviz-3.9.0/licenses/IPYFILECHOOSER_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/licenses/TEMPLATE_LICENCE.rst` & `jdaviz-3.9.0/licenses/TEMPLATE_LICENCE.rst`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/CubevizExample.ipynb` & `jdaviz-3.9.0/notebooks/CubevizExample.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/ImvizDitheredExample.ipynb` & `jdaviz-3.9.0/notebooks/ImvizDitheredExample.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976728903812238%*

 * *Differences: {"'cells'": "{33: {'source': {insert: [(10, 'my_regions = [my_aper, my_aper_sky, my_reg, "*

 * *            "my_reg_sky]\\n')], delete: [24, 22, 21, 20, 19, 18, 17, 16, 15, 14, 13, 12, 11, 10, "*

 * *            '9]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.12.0'}}"}*

```diff
@@ -335,29 +335,15 @@
                 "my_aper = CircularAperture((600, 400), r=10)\n",
                 "my_aper_sky = SkyCircularAperture(c, 1 * u.arcsec)\n",
                 "\n",
                 "# regions shape\n",
                 "my_reg = CirclePixelRegion(center=PixCoord(x=600, y=200), radius=20)\n",
                 "my_reg_sky = CircleSkyRegion(c, Angle(2, u.arcsec))\n",
                 "\n",
-                "# Numpy mask\n",
-                "idx = (np.array([350, 350, 350, 350, 350, 350, 351, 351, 351, 351, 352, 352, 352,\n",
-                "                 352, 352, 352, 352, 352, 352, 352, 353, 353, 353, 353, 353, 353,\n",
-                "                 353, 353, 353, 353, 353, 353, 354, 354, 354, 354, 354, 354, 354,\n",
-                "                 354, 355, 355, 355, 355, 355, 355, 355, 355, 356, 356, 356, 356,\n",
-                "                 356, 356, 356, 357, 357, 358, 358]),\n",
-                "       np.array([353, 354, 355, 356, 357, 358, 350, 352, 359, 361, 350, 352, 353,\n",
-                "                 354, 355, 356, 357, 358, 359, 361, 350, 351, 352, 353, 354, 355,\n",
-                "                 356, 357, 358, 359, 360, 361, 351, 352, 354, 355, 356, 357, 359,\n",
-                "                 360, 352, 353, 354, 355, 356, 357, 358, 359, 352, 353, 354, 355,\n",
-                "                 356, 357, 358, 353, 358, 352, 359]))\n",
-                "my_mask = np.zeros(data.shape, dtype=np.bool_)\n",
-                "my_mask[idx] = True\n",
-                "\n",
-                "my_regions = [my_aper, my_aper_sky, my_reg, my_reg_sky, my_mask]\n",
+                "my_regions = [my_aper, my_aper_sky, my_reg, my_reg_sky]\n",
                 "imviz.load_regions(my_regions)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "99766ca8",
             "metadata": {},
@@ -693,13 +679,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.4"
+            "version": "3.12.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `jdaviz-3.8.2/notebooks/ImvizExample.ipynb` & `jdaviz-3.9.0/notebooks/ImvizExample.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975086461089065%*

 * *Differences: {"'cells'": "{10: {'metadata': {replace: OrderedDict()}}, 34: {'source': {insert: [(10, "*

 * *            "'my_regions = [my_aper, my_aper_sky, my_reg, my_reg_sky]\\n')], delete: [24, 22, 21, "*

 * *            '20, 19, 18, 17, 16, 15, 14, 13, 12, 11, 10, 9]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.11.0'}}"}*

```diff
@@ -140,17 +140,15 @@
                 "Then, we visualize the data and start off by looking at some of the basic features:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "229d64f3-843f-4a7f-ac98-989f2a95d4c1",
-            "metadata": {
-                "scrolled": false
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "imviz.show()"
             ]
         },
         {
             "cell_type": "markdown",
@@ -382,29 +380,15 @@
                 "my_aper = CircularAperture((1714, 1380), r=20)\n",
                 "my_aper_sky = SkyCircularAperture(c, 2 * u.arcsec)\n",
                 "\n",
                 "# regions shape\n",
                 "my_reg = CirclePixelRegion(center=PixCoord(x=1526, y=1063), radius=40)\n",
                 "my_reg_sky = CircleSkyRegion(c, Angle(2, u.arcsec))\n",
                 "\n",
-                "# Numpy mask\n",
-                "idx = (np.array([350, 350, 350, 350, 350, 350, 351, 351, 351, 351, 352, 352, 352,\n",
-                "                 352, 352, 352, 352, 352, 352, 352, 353, 353, 353, 353, 353, 353,\n",
-                "                 353, 353, 353, 353, 353, 353, 354, 354, 354, 354, 354, 354, 354,\n",
-                "                 354, 355, 355, 355, 355, 355, 355, 355, 355, 356, 356, 356, 356,\n",
-                "                 356, 356, 356, 357, 357, 358, 358]),\n",
-                "       np.array([353, 354, 355, 356, 357, 358, 350, 352, 359, 361, 350, 352, 353,\n",
-                "                 354, 355, 356, 357, 358, 359, 361, 350, 351, 352, 353, 354, 355,\n",
-                "                 356, 357, 358, 359, 360, 361, 351, 352, 354, 355, 356, 357, 359,\n",
-                "                 360, 352, 353, 354, 355, 356, 357, 358, 359, 352, 353, 354, 355,\n",
-                "                 356, 357, 358, 353, 358, 352, 359]))\n",
-                "my_mask = np.zeros(data.data.shape, dtype=np.bool_)\n",
-                "my_mask[idx] = True\n",
-                "\n",
-                "my_regions = [my_aper, my_aper_sky, my_reg, my_reg_sky, my_mask]\n",
+                "my_regions = [my_aper, my_aper_sky, my_reg, my_reg_sky]\n",
                 "imviz.load_regions(my_regions)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "99766ca8",
             "metadata": {},
@@ -724,13 +708,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.10"
+            "version": "3.11.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `jdaviz-3.8.2/notebooks/MosvizExample.ipynb` & `jdaviz-3.9.0/notebooks/MosvizExample.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/MosvizNIRISSExample.ipynb` & `jdaviz-3.9.0/notebooks/MosvizNIRISSExample.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/Specviz2dExample.ipynb` & `jdaviz-3.9.0/notebooks/Specviz2dExample.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/SpecvizExample.ipynb` & `jdaviz-3.9.0/notebooks/SpecvizExample.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/concepts/cubeviz_contour_overlay.ipynb` & `jdaviz-3.9.0/notebooks/concepts/cubeviz_contour_overlay.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/concepts/cubeviz_data_interactions.ipynb` & `jdaviz-3.9.0/notebooks/concepts/cubeviz_data_interactions.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/concepts/cubeviz_fitting.ipynb` & `jdaviz-3.9.0/notebooks/concepts/cubeviz_fitting.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/concepts/cubeviz_ndarray_gif.ipynb` & `jdaviz-3.9.0/notebooks/concepts/cubeviz_ndarray_gif.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996639784946236%*

 * *Differences: {"'cells'": "{27: {'source': ['slice_plg.value = 0']}}"}*

```diff
@@ -305,15 +305,15 @@
             "execution_count": null,
             "id": "41de986e-c051-4021-a51e-bbdb6b478505",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "slice_plg.slice = 0"
+                "slice_plg.value = 0"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "7cf924c0",
             "metadata": {
```

### Comparing `jdaviz-3.8.2/notebooks/concepts/cubeviz_spectral_fitting.ipynb` & `jdaviz-3.9.0/notebooks/concepts/cubeviz_spectral_fitting.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/concepts/cubeviz_spectral_spatial_interactions.ipynb` & `jdaviz-3.9.0/notebooks/concepts/cubeviz_spectral_spatial_interactions.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/concepts/cubeviz_wfc3ir_ramp.ipynb` & `jdaviz-3.9.0/notebooks/concepts/cubeviz_wfc3ir_ramp.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/concepts/default_programmatic_viewers_from_blank.ipynb` & `jdaviz-3.9.0/notebooks/concepts/default_programmatic_viewers_from_blank.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/concepts/imviz_advanced_aper_phot.ipynb` & `jdaviz-3.9.0/notebooks/concepts/imviz_advanced_aper_phot.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/concepts/imviz_color_display.ipynb` & `jdaviz-3.9.0/notebooks/concepts/imviz_color_display.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/concepts/imviz_colorbar_mpl.ipynb` & `jdaviz-3.9.0/notebooks/concepts/imviz_colorbar_mpl.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/concepts/imviz_compass_mpl.ipynb` & `jdaviz-3.9.0/notebooks/concepts/imviz_compass_mpl.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/concepts/imviz_custom_colormap.ipynb` & `jdaviz-3.9.0/notebooks/concepts/imviz_custom_colormap.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/concepts/imviz_dithered_gwcs.ipynb` & `jdaviz-3.9.0/notebooks/concepts/imviz_dithered_gwcs.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993055555555556%*

 * *Differences: {"'cells'": '{8: {\'source\': {insert: [(1, "imviz.plugins[\'Orientation\'].link_type = '*

 * *            '\'WCS\'\\n"), (2, "imviz.plugins[\'Orientation\'].wcs_use_affine = True")], delete: '*

 * *            '[2, 1]}}}'}*

```diff
@@ -97,16 +97,16 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "fab70d10",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Link by WCS\n",
-                "imviz.plugins['Links Control'].link_type = 'WCS'\n",
-                "imviz.plugins['Links Control'].wcs_use_affine = True"
+                "imviz.plugins['Orientation'].link_type = 'WCS'\n",
+                "imviz.plugins['Orientation'].wcs_use_affine = True"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "6e7d1198",
             "metadata": {},
```

### Comparing `jdaviz-3.8.2/notebooks/concepts/imviz_edit_subset_programmatic.ipynb` & `jdaviz-3.9.0/notebooks/concepts/imviz_edit_subset_programmatic.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/concepts/imviz_line_profiles.ipynb` & `jdaviz-3.9.0/notebooks/concepts/imviz_line_profiles.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/concepts/imviz_load_3d_slices.ipynb` & `jdaviz-3.9.0/notebooks/concepts/imviz_load_3d_slices.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/concepts/imviz_load_fits_hdu.ipynb` & `jdaviz-3.9.0/notebooks/concepts/imviz_load_fits_hdu.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/concepts/imviz_roman_asdf.ipynb` & `jdaviz-3.9.0/notebooks/concepts/imviz_roman_asdf.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9870231331168831%*

 * *Differences: {"'cells'": "{6: {'source': {insert: [(0, 'from astropy.utils.data import download_file\\n'), (2, "*

 * *            '\'# # Each of these files is ~1 GB:\\n\'), (3, "image_model1 = '*

 * *            "download_file('https://stsci.box.com/shared/static/be2nfy4jovdhw1cxru99kdwnfnqxxlgo.asdf', "*

 * *            'cache=True)\\n"), (4, "image_model2 = '*

 * *            "download_file('https://stsci.box.com/shared/static/ktpt4li627kq4mipi3er5yd4qw6hq7ll.asdf', "*

 * *            'cache=True)")], delete: [2, 0]}}, 7: {\'source\': {inser […]*

```diff
@@ -66,17 +66,19 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "68443a20",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from astropy.utils.data import get_pkg_data_filename\n",
+                "from astropy.utils.data import download_file\n",
                 "\n",
-                "image_model = get_pkg_data_filename('data/roman_wfi_image_model.asdf', package='jdaviz.configs.imviz.tests')"
+                "# # Each of these files is ~1 GB:\n",
+                "image_model1 = download_file('https://stsci.box.com/shared/static/be2nfy4jovdhw1cxru99kdwnfnqxxlgo.asdf', cache=True)\n",
+                "image_model2 = download_file('https://stsci.box.com/shared/static/ktpt4li627kq4mipi3er5yd4qw6hq7ll.asdf', cache=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "6fb39d1e-7b10-4e9f-8d42-1d971b035014",
             "metadata": {
@@ -85,15 +87,16 @@
             "outputs": [],
             "source": [
                 "# load the observations into the helper\n",
                 "imviz = Imviz()\n",
                 "\n",
                 "with warnings.catch_warnings():\n",
                 "    warnings.simplefilter('ignore')  # ErfaWarning\n",
-                "    imviz.load_data(image_model, ext='data')"
+                "    imviz.load_data(image_model1, ext='data', data_label='exposure 1')\n",
+                "    imviz.load_data(image_model2, ext='data', data_label='exposure 2')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e28b9919-6f9e-410c-83f6-554631407d4b",
             "metadata": {},
             "source": [
@@ -103,15 +106,35 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "229d64f3-843f-4a7f-ac98-989f2a95d4c1",
             "metadata": {},
             "outputs": [],
             "source": [
-                "imviz.show()"
+                "imviz.show('sidecar:split-right', height=1000)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "52adc3d4-7f44-43aa-af46-6acb390d56e2",
+            "metadata": {},
+            "source": [
+                "We have loaded two sequential exposures with the same pointing. Let's orient both images by their WCS:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "8427d4f9-8ea3-4d60-a8b7-3f3f63e3f3e0",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "orientation = imviz.plugins['Orientation']\n",
+                "\n",
+                "orientation.link_type = 'WCS'"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "1abb759e",
             "metadata": {},
             "source": [
@@ -125,24 +148,28 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "f117ebce-c7a0-44fa-82a4-0c0876663093",
             "metadata": {},
             "outputs": [],
             "source": [
+                "plot_options = imviz.plugins['Plot Options']\n",
+                "\n",
                 "for viewer_name in imviz.app.get_viewer_reference_names():\n",
                 "    viewer = imviz.app.get_viewer(viewer_name)\n",
-                "\n",
-                "    # set colormap and stretch:\n",
-                "    viewer.stretch = 'log'\n",
-                "    viewer.set_colormap('Viridis')\n",
-                "    viewer.cuts = [1, 1e4]\n",
+                "    plot_options.viewer = viewer_name\n",
                 "    \n",
-                "    # set zoom level\n",
-                "    viewer.zoom(1.25)"
+                "    for data in viewer.data():\n",
+                "        plot_options.layer = data.label\n",
+                "        \n",
+                "        # set colormap and stretch for this layer:\n",
+                "        plot_options.stretch_function = 'arcsinh'\n",
+                "        plot_options.image_colormap = 'Viridis'\n",
+                "        plot_options.stretch_vmin = 0\n",
+                "        plot_options.stretch_vmax = 20"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "2f25ccd8",
             "metadata": {},
             "source": [
@@ -188,15 +215,16 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "71e2191b",
             "metadata": {},
             "outputs": [],
             "source": [
-                "mask = regions['Subset 1'].to_mask(mode='subpixels')"
+                "wcs = imviz.app.data_collection[-1].coords\n",
+                "mask = regions['Subset 1'].to_pixel(wcs).to_mask(mode='subpixels')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "0a4e02ef",
             "metadata": {},
@@ -222,14 +250,24 @@
             "source": [
                 "You can use Astrowidgets API."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "f2ce00c9-093c-4bc0-8cb7-b7c8fe38ec64",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "viewer = imviz.default_viewer"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
             "id": "5e908421",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Center the image on given pixel position.\n",
                 "viewer.center_on((6, 5))  # X, Y (0-indexed)"
             ]
@@ -256,27 +294,26 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "05bc5603-9815-433f-8b4b-2556222ce6c5",
             "metadata": {},
             "outputs": [],
             "source": [
-                "center = regions['Subset 1'].center\n",
-                "data.wcs.pixel_to_world([center.x], [center.y]).to_string('hmsdms')"
+                "center = regions['Subset 1'].center"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e0f3845a",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Center the image on given sky coordinates.\n",
-                "sky = SkyCoord(ra=\"13h11m34.25069521s\", dec=\"-01d21m55.92127995s\")\n",
+                "sky = SkyCoord(ra=79.91038, dec=29.95529, unit=('deg', 'deg'))\n",
                 "viewer.center_on(sky)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "20f51452-1858-47f9-a421-2997f54f8433",
@@ -317,26 +354,26 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "7a834bcf-7d5a-492b-bc54-740e1500a2f4",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Set the zoom level directly.\n",
-                "viewer.zoom_level = 1"
+                "viewer.zoom_level = 100"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "32288b81-1817-4549-b2e4-5e7f55b0ee3d",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Set the relative zoom based on current zoom level.\n",
-                "viewer.zoom(2)"
+                "viewer.zoom(1.5)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "11fab067-7428-4ce4-bc9b-f5462fe52e2a",
             "metadata": {},
             "source": [
@@ -351,38 +388,29 @@
             "outputs": [],
             "source": [
                 "# Add 20 randomly generated X,Y (0-indexed) w.r.t. reference image\n",
                 "# using default marker properties.\n",
                 "image_shape = data.data.shape\n",
                 "t_xy = Table({'x': np.random.randint(0, image_shape[1], 20),\n",
                 "              'y': np.random.randint(0, image_shape[0], 20)})\n",
+                "\n",
                 "viewer.add_markers(t_xy)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f1c1aa0d-46b7-42f6-b6d7-395305c15f91",
             "metadata": {},
             "source": [
                 "You could customize marker color, alpha, size, and fill with values that Glue supports."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "7c8edb6f-c928-4aee-8e64-73a34ab020d0",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "viewer.marker = {'color': 'green', 'alpha': 0.8, 'markersize': 10, 'fill': False}"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
             "id": "9ecfd0f9-da9e-419b-99a8-cc6efc20568f",
             "metadata": {},
             "outputs": [],
             "source": [
                 "np.random.seed(42)\n",
                 "# Mark some sky coordinates using updated marker properties.\n",
                 "t_sky = Table({'coord': [sky.spherical_offsets_by(*np.random.normal(scale=0.1, size=2) * u.arcsec)\n",
@@ -484,15 +512,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "77368ba8",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Show the first image in the second viewer.\n",
-                "imviz.app.add_data_to_viewer(viewer_2_name, \"roman_wfi_image_model[DATA]\")"
+                "imviz.app.add_data_to_viewer(viewer_2_name, \"exposure 1[DATA]\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "448f72f8-eb53-4c45-9afc-54dc69a9798f",
             "metadata": {},
@@ -514,15 +542,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "74c81ca4",
             "metadata": {},
             "outputs": [],
             "source": [
-                "viewer_2.center_on((5, 1))"
+                "viewer_2.center_on((1500, 1000))"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "8194c11e-f947-489f-9484-f85863f23797",
             "metadata": {},
             "source": [
@@ -560,13 +588,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.8"
+            "version": "3.11.5"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `jdaviz-3.8.2/notebooks/concepts/imviz_simple_aper_phot.ipynb` & `jdaviz-3.9.0/notebooks/concepts/imviz_simple_aper_phot.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/concepts/mosviz_concept.ipynb` & `jdaviz-3.9.0/notebooks/concepts/mosviz_concept.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/concepts/mosviz_generate_photometry.ipynb` & `jdaviz-3.9.0/notebooks/concepts/mosviz_generate_photometry.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/concepts/mosviz_niriss_parser.ipynb` & `jdaviz-3.9.0/notebooks/concepts/mosviz_niriss_parser.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/concepts/pypi_metrics.ipynb` & `jdaviz-3.9.0/notebooks/concepts/pypi_metrics.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/concepts/specviz_from_list.ipynb` & `jdaviz-3.9.0/notebooks/concepts/specviz_from_list.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/concepts/specviz_from_splot.ipynb` & `jdaviz-3.9.0/notebooks/concepts/specviz_from_splot.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/concepts/specviz_glue_unit_conversion.ipynb` & `jdaviz-3.9.0/notebooks/concepts/specviz_glue_unit_conversion.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/concepts/specviz_line_lists.ipynb` & `jdaviz-3.9.0/notebooks/concepts/specviz_line_lists.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/concepts/specviz_minimal.ipynb` & `jdaviz-3.9.0/notebooks/concepts/specviz_minimal.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/notebooks/concepts/specviz_spectrum_list.ipynb` & `jdaviz-3.9.0/notebooks/concepts/specviz_spectrum_list.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/pyproject.toml` & `jdaviz-3.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,15 @@
     "\"jdaviz\"",
     "\"docs\"",
 ]
 astropy_header = true
 doctest_plus = "enabled"
 text_file_format = "rst"
 addopts = "--doctest-rst --import-mode=append"
+xfail_strict = true
 filterwarnings = [
     "error",
     "ignore:numpy\\.ufunc size changed:RuntimeWarning",
     "ignore:numpy\\.ndarray size changed:RuntimeWarning",
     "ignore:Passing unrecognized arguments to super:DeprecationWarning",
     "ignore:.*With traitlets 4\\.1, metadata should be set using the \\.tag\\(\\) method:DeprecationWarning",
     "ignore:The unit 'Angstrom' has been deprecated in the VOUnit standard\\. Suggested.* 0\\.1nm\\.",
@@ -143,22 +144,22 @@
 
 [tool.coverage.run]
 omit = [
     "jdaviz/_astropy_init*",
     "jdaviz/conftest.py",
     "jdaviz/*setup_package*",
     "jdaviz/tests/*",
-    "jdaviz/*/tests/*",
+    "jdaviz/**/tests/*",
     "jdaviz/extern/*",
     "jdaviz/version*",
     "*/jdaviz/_astropy_init*",
     "*/jdaviz/conftest.py",
     "*/jdaviz/*setup_package*",
     "*/jdaviz/tests/*",
-    "*/jdaviz/*/tests/*",
+    "*/jdaviz/**/tests/*",
     "*/jdaviz/extern/*",
     "*/jdaviz/version*",
 ]
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
```

### Comparing `jdaviz-3.8.2/setup.py` & `jdaviz-3.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/share/jupyter/nbconvert/templates/jdaviz-default/ansi.js` & `jdaviz-3.9.0/share/jupyter/nbconvert/templates/jdaviz-default/ansi.js`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/share/jupyter/nbconvert/templates/jdaviz-default/app.html` & `jdaviz-3.9.0/share/jupyter/nbconvert/templates/jdaviz-default/app.html`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/share/jupyter/nbconvert/templates/jdaviz-default/index.html.j2` & `jdaviz-3.9.0/share/jupyter/nbconvert/templates/jdaviz-default/index.html.j2`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/share/jupyter/nbconvert/templates/jdaviz-default/util.js` & `jdaviz-3.9.0/share/jupyter/nbconvert/templates/jdaviz-default/util.js`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/share/jupyter/voila/templates/jdaviz-default/index.html.j2` & `jdaviz-3.9.0/share/jupyter/voila/templates/jdaviz-default/index.html.j2`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/standalone/jdaviz-cli-entrypoint.py` & `jdaviz-3.9.0/standalone/jdaviz-cli-entrypoint.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/standalone/jdaviz.spec` & `jdaviz-3.9.0/standalone/jdaviz.spec`

 * *Files identical despite different names*

### Comparing `jdaviz-3.8.2/tox.ini` & `jdaviz-3.9.0/tox.ini`

 * *Files identical despite different names*

