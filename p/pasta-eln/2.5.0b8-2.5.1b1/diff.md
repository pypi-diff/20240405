# Comparing `tmp/pasta_eln-2.5.0b8.tar.gz` & `tmp/pasta_eln-2.5.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasta_eln-2.5.0b8.tar", last modified: Mon Mar 25 12:45:06 2024, max compression
+gzip compressed data, was "pasta_eln-2.5.1b1.tar", last modified: Fri Apr  5 09:17:15 2024, max compression
```

## Comparing `pasta_eln-2.5.0b8.tar` & `pasta_eln-2.5.1b1.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:45:06.739945 pasta_eln-2.5.0b8/
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-03-25 12:45:06.739945 pasta_eln-2.5.0b8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/README_PYPI.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:45:06.703945 pasta_eln-2.5.0b8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:45:06.703945 pasta_eln-2.5.0b8/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:45:06.711944 pasta_eln-2.5.0b8/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)  2003429 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/docs/source/_static/Data_Hierarchy_Editor_Manual.odp
--rw-r--r--   0 runner    (1001) docker     (127)  1695262 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/docs/source/_static/Data_Hierarchy_Editor_Manual.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/docs/source/_static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   225801 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/docs/source/_static/data_hierarchy_editor.png
--rw-r--r--   0 runner    (1001) docker     (127)   985134 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/docs/source/_static/metadata_group_combobox.png
--rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/docs/source/_static/pasta_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   100504 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/docs/source/_static/pyside.png
--rw-r--r--   0 runner    (1001) docker     (127)   846253 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/docs/source/_static/types_combo_box.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:45:06.699944 pasta_eln-2.5.0b8/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:45:06.711944 pasta_eln-2.5.0b8/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/docs/source/data_hierarchy_configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/docs/source/dodonts.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9683 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/docs/source/extractors.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/docs/source/faqs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/docs/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11238 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/docs/source/motivation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/docs/source/userstory.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:45:06.715944 pasta_eln-2.5.0b8/pasta_eln/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:45:06.719944 pasta_eln-2.5.0b8/pasta_eln/Extractors/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/Extractors/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/Extractors/extractor_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/Extractors/extractor_jpeg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/Extractors/extractor_jpg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/Extractors/extractor_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/Extractors/extractor_md.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/Extractors/extractor_png.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/Extractors/extractor_py.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:45:06.719944 pasta_eln-2.5.0b8/pasta_eln/GUI/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/_contextMenu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/body.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/configAuthors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/configGUI.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/configSetupLinux.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6826 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/configSetupWindows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:45:06.727944 pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/attachments_tableview_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/create_type_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)    23214 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    21471 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21656 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/delete_column_delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/document_null_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/generic_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/iri_column_delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/key_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/lookup_iri_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/mandatory_column_delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/metadata_tableview_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/reorder_column_delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7616 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/tableview_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/terminology_lookup_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/terminology_lookup_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    19014 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:45:06.731944 pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/completed_upload_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/completed_upload_task.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/completed_uploads.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/completed_uploads_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/completed_uploads_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/config_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/config_dialog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8740 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/config_dialog_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)     7415 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/controlled_vocab_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/dialog_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/edit_metadata_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/main_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/main_dialog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/main_dialog_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)    21062 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/primitive_compound_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/project_item_frame_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/project_item_frame_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/upload_config_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/upload_config_dialog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/upload_config_dialog_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/upload_widget_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/upload_widget_base.ui
--rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/details.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/docTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    29036 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/form.py
--rw-r--r--   0 runner    (1001) docker     (127)    18601 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/projectGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/projectLeafRenderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/projectTreeView.py
--rw-r--r--   0 runner    (1001) docker     (127)     9559 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/sidebar.py
--rw-r--r--   0 runner    (1001) docker     (127)    19430 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/GUI/tableHeader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:45:06.699944 pasta_eln-2.5.0b8/pasta_eln/Resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:45:06.731944 pasta_eln-2.5.0b8/pasta_eln/Resources/ExampleMeasurements/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/Resources/ExampleMeasurements/simple.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/Resources/ExampleMeasurements/simple.png
--rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/Resources/ExampleMeasurements/story.odt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:45:06.731944 pasta_eln-2.5.0b8/pasta_eln/Resources/Icons/
--rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/Resources/Icons/favicon64.ico
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/Resources/Icons/favicon64.png
--rw-r--r--   0 runner    (1001) docker     (127)    20226 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/Resources/Icons/ols.png
--rw-r--r--   0 runner    (1001) docker     (127)    17206 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/Resources/Icons/tib.png
--rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/Resources/Icons/wikidata.png
--rw-r--r--   0 runner    (1001) docker     (127)    17310 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/Resources/Icons/wikipedia.png
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35306 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/backend.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14107 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    44043 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:45:06.735944 pasta_eln-2.5.0b8/pasta_eln/dataverse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/dataverse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12850 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/dataverse/base_database_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/dataverse/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    31059 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/dataverse/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/dataverse/config_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/dataverse/config_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/dataverse/data_upload_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/dataverse/database_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/dataverse/database_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    49819 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/dataverse/dataset-create-new-all-default-fields.json
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/dataverse/generic_task_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/dataverse/incorrect_parameter_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/dataverse/project_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/dataverse/task_thread_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)    10671 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/dataverse/upload_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/dataverse/upload_queue_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/dataverse/upload_status_values.py
--rw-r--r--   0 runner    (1001) docker     (127)    21590 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/dataverse/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    29213 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/fixedStringsJson.py
--rw-r--r--   0 runner    (1001) docker     (127)    11775 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/guiCommunicate.py
--rw-r--r--   0 runner    (1001) docker     (127)    13007 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/guiStyle.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8582 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/handleDictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)    23440 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/inputOutput.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21832 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/installationTools.py
--rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/miscTools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/mixin_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/printer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23148 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/serverActions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:45:06.735944 pasta_eln-2.5.0b8/pasta_eln/webclient/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/webclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pasta_eln/webclient/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:45:06.735944 pasta_eln-2.5.0b8/pasta_eln.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-03-25 12:45:06.000000 pasta_eln-2.5.0b8/pasta_eln.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-03-25 12:45:06.000000 pasta_eln-2.5.0b8/pasta_eln.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 12:45:06.000000 pasta_eln-2.5.0b8/pasta_eln.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-25 12:45:06.000000 pasta_eln-2.5.0b8/pasta_eln.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-25 12:45:06.000000 pasta_eln-2.5.0b8/pasta_eln.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-25 12:45:06.000000 pasta_eln-2.5.0b8/pasta_eln.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-03-25 12:45:06.739945 pasta_eln-2.5.0b8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-03-25 12:45:06.000000 pasta_eln-2.5.0b8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:45:06.735944 pasta_eln-2.5.0b8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/tests/test_01_3Projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/tests/test_02_3Projects_ExportImport.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/tests/test_50_importOthers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-03-25 12:45:00.000000 pasta_eln-2.5.0b8/tests/test_99_3Projects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.634384 pasta_eln-2.5.1b1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-05 09:17:15.634384 pasta_eln-2.5.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/README_PYPI.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.598384 pasta_eln-2.5.1b1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.602384 pasta_eln-2.5.1b1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.610384 pasta_eln-2.5.1b1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)  2003429 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/_static/Data_Hierarchy_Editor_Manual.odp
+-rw-r--r--   0 runner    (1001) docker     (127)  1695262 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/_static/Data_Hierarchy_Editor_Manual.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/_static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   225801 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/_static/data_hierarchy_editor.png
+-rw-r--r--   0 runner    (1001) docker     (127)   985134 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/_static/metadata_group_combobox.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/_static/pasta_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   100504 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/_static/pyside.png
+-rw-r--r--   0 runner    (1001) docker     (127)   846253 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/_static/types_combo_box.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.598384 pasta_eln-2.5.1b1/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.610384 pasta_eln-2.5.1b1/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/data_hierarchy_configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/dodonts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9683 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/extractors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/faqs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11238 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/motivation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/docs/source/userstory.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.614384 pasta_eln-2.5.1b1/pasta_eln/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.614384 pasta_eln-2.5.1b1/pasta_eln/Extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Extractors/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Extractors/extractor_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Extractors/extractor_jpeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Extractors/extractor_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Extractors/extractor_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Extractors/extractor_md.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Extractors/extractor_png.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Extractors/extractor_py.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.618384 pasta_eln-2.5.1b1/pasta_eln/GUI/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/_contextMenu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/configAuthors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/configGUI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/configSetupLinux.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7874 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/configSetupWindows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.622384 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/attachments_tableview_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/create_type_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    23214 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21471 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21656 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/delete_column_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/document_null_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/generic_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/iri_column_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/key_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/lookup_iri_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/mandatory_column_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/metadata_tableview_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/reorder_column_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7616 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/tableview_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19014 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.626384 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/completed_upload_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/completed_upload_task.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/completed_uploads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/completed_uploads_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/completed_uploads_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/config_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/config_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8740 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/config_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     7415 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/controlled_vocab_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/dialog_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/edit_metadata_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/main_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/main_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/main_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    21062 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/primitive_compound_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/project_item_frame_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/project_item_frame_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/upload_config_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/upload_config_dialog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/upload_config_dialog_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/upload_widget_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/upload_widget_base.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/docTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29145 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18963 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/projectGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/projectLeafRenderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8566 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/projectTreeView.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9559 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/sidebar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19456 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/GUI/tableHeader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.598384 pasta_eln-2.5.1b1/pasta_eln/Resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.626384 pasta_eln-2.5.1b1/pasta_eln/Resources/ExampleMeasurements/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Resources/ExampleMeasurements/simple.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Resources/ExampleMeasurements/simple.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Resources/ExampleMeasurements/story.odt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.626384 pasta_eln-2.5.1b1/pasta_eln/Resources/Icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Resources/Icons/favicon64.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Resources/Icons/favicon64.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20226 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Resources/Icons/ols.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17206 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Resources/Icons/tib.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Resources/Icons/wikidata.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17310 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/Resources/Icons/wikipedia.png
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35774 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/backend.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14107 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43862 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.630384 pasta_eln-2.5.1b1/pasta_eln/dataverse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12850 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/base_database_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31059 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/config_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/config_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/data_upload_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/database_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/database_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49819 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/dataset-create-new-all-default-fields.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/generic_task_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/incorrect_parameter_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/project_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/task_thread_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10671 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/upload_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/upload_queue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/upload_status_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21590 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/dataverse/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29213 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/fixedStringsJson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11775 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/guiCommunicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13007 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/guiStyle.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8622 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/handleDictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23440 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/inputOutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22498 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/installationTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/miscTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/mixin_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/printer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23450 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/serverActions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.630384 pasta_eln-2.5.1b1/pasta_eln/webclient/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/webclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pasta_eln/webclient/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.630384 pasta_eln-2.5.1b1/pasta_eln.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-05 09:17:15.000000 pasta_eln-2.5.1b1/pasta_eln.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-04-05 09:17:15.000000 pasta_eln-2.5.1b1/pasta_eln.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 09:17:15.000000 pasta_eln-2.5.1b1/pasta_eln.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-05 09:17:15.000000 pasta_eln-2.5.1b1/pasta_eln.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-05 09:17:15.000000 pasta_eln-2.5.1b1/pasta_eln.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 09:17:15.000000 pasta_eln-2.5.1b1/pasta_eln.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-05 09:17:15.634384 pasta_eln-2.5.1b1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-04-05 09:17:15.000000 pasta_eln-2.5.1b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:17:15.630384 pasta_eln-2.5.1b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/tests/test_01_3Projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/tests/test_02_3Projects_ExportImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/tests/test_50_importOthers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-04-05 09:17:10.000000 pasta_eln-2.5.1b1/tests/test_99_3Projects.py
```

### Comparing `pasta_eln-2.5.0b8/LICENSE` & `pasta_eln-2.5.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/PKG-INFO` & `pasta_eln-2.5.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasta_eln
-Version: 2.5.0b8
+Version: 2.5.1b1
 Summary: The favorite ELN for experimental scientists
 Home-page: https://pasta-eln.github.io/
 Author: The PASTA-ELN Team and Steffen Brinckmann
 Author-email: sbrinckm@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pasta_eln-2.5.0b8/README.md` & `pasta_eln-2.5.1b1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -125,10 +125,20 @@
 doc = backend.db.getDoc("m-3a43570c4fd84b1ab81a8863ae058fb0")
 dialog = Form(comm, doc)
 dialog.show()
 sys.exit(app.exec())
 ```
 and execute "python -m pasta_eln.test"
 
+#### Profiling
+Begin...
+      from cProfile import Profile
+      from pstats import SortKey, Stats
+      with Profile() as profile:
+
+End...
+      (Stats(profile).strip_dirs().sort_stats(SortKey.CUMULATIVE).print_stats()) #end cProfile
+
+
 #### General notes
 - Find qt-awesome icons: qta-browser
 - print works great in frondend and backend
```

### Comparing `pasta_eln-2.5.0b8/README_PYPI.md` & `pasta_eln-2.5.1b1/README_PYPI.md`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/docs/Makefile` & `pasta_eln-2.5.1b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/docs/README.md` & `pasta_eln-2.5.1b1/docs/README.md`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/docs/source/_static/Data_Hierarchy_Editor_Manual.odp` & `pasta_eln-2.5.1b1/docs/source/_static/Data_Hierarchy_Editor_Manual.odp`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/docs/source/_static/Data_Hierarchy_Editor_Manual.pdf` & `pasta_eln-2.5.1b1/docs/source/_static/Data_Hierarchy_Editor_Manual.pdf`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/docs/source/_static/data_hierarchy_editor.png` & `pasta_eln-2.5.1b1/docs/source/_static/data_hierarchy_editor.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/docs/source/_static/metadata_group_combobox.png` & `pasta_eln-2.5.1b1/docs/source/_static/metadata_group_combobox.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/docs/source/_static/pasta_logo.svg` & `pasta_eln-2.5.1b1/docs/source/_static/pasta_logo.svg`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/docs/source/_static/pyside.png` & `pasta_eln-2.5.1b1/docs/source/_static/pyside.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/docs/source/_static/types_combo_box.png` & `pasta_eln-2.5.1b1/docs/source/_static/types_combo_box.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/docs/source/conf.py` & `pasta_eln-2.5.1b1/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 project = u'PASTA-ELN'
 copyright = u'2022-{}, PASTA-ELN team'.format(datetime.datetime.now().year)
 author = u'PASTA-ELN team'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
-version = "2.5.0b7"
+version = "2.5.0"
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
```

### Comparing `pasta_eln-2.5.0b8/docs/source/data_hierarchy_configuration.rst` & `pasta_eln-2.5.1b1/docs/source/data_hierarchy_configuration.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/docs/source/dodonts.rst` & `pasta_eln-2.5.1b1/docs/source/dodonts.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/docs/source/extractors.rst` & `pasta_eln-2.5.1b1/docs/source/extractors.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/docs/source/faqs.rst` & `pasta_eln-2.5.1b1/docs/source/faqs.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/docs/source/index.rst` & `pasta_eln-2.5.1b1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/docs/source/install.rst` & `pasta_eln-2.5.1b1/docs/source/install.rst`

 * *Files 8% similar despite different names*

```diff
@@ -6,20 +6,28 @@
 WINDOWS
 =======
 
 Install python via Anaconda and then PASTA-ELN
 ----------------------------------------------
 
 If you do not have Python installed, we recommend using Anaconda.
-1. Go to https://www.anaconda.com/download
-2. Download installer and run install. Accept all defaults
-3. Create environment, e.g. PASTA-ELN
-4. Open environment in command-prompt
-5. "pip install pasta-eln"
-6. "python -m pasta_eln.gui"
+1. Be sure that .NET version 3.5 is installed.
+
+   https://learn.microsoft.com/en-us/dotnet/framework/install/dotnet-35-windows
+
+2. Go to https://www.anaconda.com/download
+3. Download installer and run install. Accept all defaults
+4. Create environment, e.g. PASTA-ELN and choose to install it with "Python 3.11..."
+5. Click on new green arrow button and open "Terminal"
+6. "pip install pasta-eln"
+7. "pip install pasta-eln -U --no-dependencies"
+
+    - if it complains about 'aiohttp' missing "pip install aiohttp"
+
+8. "python -m pasta_eln.gui" (make sure that you have administrator rights)
 
 
 Manual installation
 ^^^^^^^^^^^^^^^^^^^
 
 If automatic installation fails
 1. Manually install couchdb https://docs.couchdb.org/en/stable/install/windows.html
```

### Comparing `pasta_eln-2.5.0b8/docs/source/motivation.rst` & `pasta_eln-2.5.1b1/docs/source/motivation.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/docs/source/userstory.rst` & `pasta_eln-2.5.1b1/docs/source/userstory.rst`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/Extractors/extractor_csv.py` & `pasta_eln-2.5.1b1/pasta_eln/Extractors/extractor_csv.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/Extractors/extractor_jpeg.py` & `pasta_eln-2.5.1b1/pasta_eln/Extractors/extractor_jpeg.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/Extractors/extractor_jpg.py` & `pasta_eln-2.5.1b1/pasta_eln/Extractors/extractor_jpg.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/Extractors/extractor_json.py` & `pasta_eln-2.5.1b1/pasta_eln/Extractors/extractor_json.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/Extractors/extractor_md.py` & `pasta_eln-2.5.1b1/pasta_eln/Extractors/extractor_md.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/Extractors/extractor_png.py` & `pasta_eln-2.5.1b1/pasta_eln/Extractors/extractor_png.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/Extractors/extractor_py.py` & `pasta_eln-2.5.1b1/pasta_eln/Extractors/extractor_py.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/_contextMenu.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/_contextMenu.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/body.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/body.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/config.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/config.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/configAuthors.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/configAuthors.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/configGUI.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/configGUI.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/configSetupLinux.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/configSetupLinux.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/configSetupWindows.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/configSetupWindows.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ Widget: setup tab inside the configuration dialog window """
-import logging
+import logging, os, ctypes
 from enum import Enum
 from pathlib import Path
 from typing import Callable, Any
 from PySide6.QtWidgets import QWidget, QVBoxLayout, QTextEdit, QMessageBox, QFileDialog, QProgressBar   # pylint: disable=no-name-in-module
 from ..guiStyle import TextButton, widgetAndLayout
-from ..installationTools import couchdb, configuration, dataHierarchy, exampleData, createShortcut
+from ..installationTools import couchdb, configuration, dataHierarchy, exampleData, createShortcut, checkForDotNetVersion
 from ..fixedStringsJson import setupTextWindows, couchDBWindows, exampleDataWindows, restartPastaWindows
 from ..miscTools import restart
 from ..guiCommunicate import Communicate
 
 class ConfigurationSetup(QWidget):
   """
   Main class
@@ -72,20 +72,37 @@
         res = couchdb('test')
         if res =='':
           self.mainText = self.mainText.replace('- CouchDB','- CouchDB is installed' )
           self.text1.setMarkdown(self.mainText)
         else:
           button = QMessageBox.question(self, "CouchDB installation", couchDBWindows)
           if button == QMessageBox.Yes:
-            res = couchdb('install')
-            flagInstalledSoftware = True
-            if len(res.split('|'))==3:
-              password=res.split('|')[1]
+            try:
+              isAdmin = os.getuid() == 0
+            except AttributeError:
+              isAdmin = ctypes.windll.shell32.IsUserAnAdmin() == 1 # type: ignore[attr-defined]
+            if not isAdmin:
+              QMessageBox.information(self,'Administrator rights required', \
+                          'You require administrator rights for your user. I exit installation now.')
+              self.mainText = self.mainText.replace('- CouchDB','- CouchDB: no admin rights' )
+              self.text1.setMarkdown(self.mainText)
+              flagContinue = False
+            elif not checkForDotNetVersion():
+              QMessageBox.information(self,'.NET version 3.5 required', \
+                          '.NET version 3.5 is required for the installation of couchDB. I exit installation now.')
+              self.mainText = self.mainText.replace('- CouchDB','- CouchDB: no .NET 3.5' )
+              self.text1.setMarkdown(self.mainText)
+              flagContinue = False
             else:
-              logging.error('Could not retrieve password :%s',str(res))
+              res = couchdb('install')
+              flagInstalledSoftware = True
+              if len(res.split('|'))==3:
+                password=res.split('|')[1]
+              else:
+                logging.error('Could not retrieve password :%s',str(res))
           else:
             self.mainText = self.mainText.replace('- CouchDB','- CouchDB: user chose to NOT install' )
             self.text1.setMarkdown(self.mainText)
             flagContinue = False
 
       #Configuration
       if flagContinue:
@@ -127,15 +144,15 @@
           self.mainText = self.mainText.replace('- Shortcut creation', '- User selected to add a shortcut' )
         else:
           self.mainText = self.mainText.replace('- Shortcut creation', '- User selected to NOT add a shortcut' )
         self.text1.setMarkdown(self.mainText)
 
       #If installed, restart
       if flagInstalledSoftware:
-        button = QMessageBox.information(self,'PASTA-ELN restart required', restartPastaWindows)
+        QMessageBox.information(self,'PASTA-ELN restart required', restartPastaWindows)
         restart()
 
       #Example data
       if flagContinue:
         button = QMessageBox.question(self, "Example data", exampleDataWindows)
         if button == QMessageBox.Yes:
           self.progress1.show()
@@ -160,12 +177,11 @@
     elif command[0] is Command.FINISHED: # What do do when setup is finished: success or unsuccessfully
       restart()
       # self.callbackFinished()
     return
 
 
 
-
 class Command(Enum):
   """ Commands used in this file """
   ANALYSE   = 1
   FINISHED  = 2
```

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/attachments_tableview_data_model.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/attachments_tableview_data_model.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/constants.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/constants.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/create_type_dialog.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/create_type_dialog.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.ui` & `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/create_type_dialog_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.ui` & `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/data_hierarchy_editor_dialog_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/delete_column_delegate.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/delete_column_delegate.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/document_null_exception.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/document_null_exception.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/generic_exception.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/generic_exception.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/iri_column_delegate.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/iri_column_delegate.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/key_not_found_exception.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/key_not_found_exception.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/lookup_iri_action.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/lookup_iri_action.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/mandatory_column_delegate.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/mandatory_column_delegate.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/metadata_tableview_data_model.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/metadata_tableview_data_model.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/reorder_column_delegate.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/reorder_column_delegate.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/tableview_data_model.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/tableview_data_model.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/terminology_lookup_config.json` & `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_config.json`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.ui` & `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_dialog_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/terminology_lookup_service.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/terminology_lookup_service.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/data_hierarchy/utility_functions.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/data_hierarchy/utility_functions.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/completed_upload_task.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/completed_upload_task.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/completed_upload_task.ui` & `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/completed_upload_task.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/completed_uploads.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/completed_uploads.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/completed_uploads_base.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/completed_uploads_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/completed_uploads_base.ui` & `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/completed_uploads_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/config_dialog.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/config_dialog.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/config_dialog_base.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/config_dialog_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/config_dialog_base.ui` & `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/config_dialog_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/controlled_vocab_frame.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/controlled_vocab_frame.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/dialog_extension.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/dialog_extension.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/edit_metadata_dialog.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/edit_metadata_dialog.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.ui` & `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/edit_metadata_dialog_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/main_dialog.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/main_dialog.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/main_dialog_base.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/main_dialog_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/main_dialog_base.ui` & `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/main_dialog_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.ui` & `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/primitive_compound_controlled_frame_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/primitive_compound_frame.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/primitive_compound_frame.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/project_item_frame_base.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/project_item_frame_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/project_item_frame_base.ui` & `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/project_item_frame_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/upload_config_dialog.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/upload_config_dialog.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/upload_config_dialog_base.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/upload_config_dialog_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/upload_config_dialog_base.ui` & `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/upload_config_dialog_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/upload_widget_base.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/upload_widget_base.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/dataverse/upload_widget_base.ui` & `pasta_eln-2.5.1b1/pasta_eln/GUI/dataverse/upload_widget_base.ui`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/details.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/details.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
   def __init__(self, comm:Communicate):
     super().__init__()
     self.comm = comm
     comm.changeDetails.connect(self.change)
     comm.testExtractor.connect(self.testExtractor)
     self.doc:dict[str,Any]  = {}
     self.docID= ''
+    self.rescaleTexts:list[QTextEdit] = []
 
     # GUI elements
     self.mainW, self.mainL = widgetAndLayout('V', None)
     self.setVerticalScrollBarPolicy(Qt.ScrollBarAlwaysOn)
     self.setHorizontalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
     self.setWidgetResizable(True)
     self.setWidget(self.mainW)
@@ -82,14 +83,15 @@
     self.metaVendorW.hide()
     self.metaUserW.hide()
     self.metaDatabaseW.hide()
     self.btnDetails.setChecked(True)
     self.btnVendor.setChecked(True)
     self.btnUser.setChecked(True)
     self.btnDatabase.setChecked(False)
+    self.rescaleTexts = []
     if not docID:  #if given '' docID, return
       return
     # Create new
     if docID!='redraw':
       self.docID = docID
     if self.docID=='':
       return
@@ -151,24 +153,25 @@
         label.setText(cssStyle+dict2ul(self.doc[key]))
         label.setTextInteractionFlags(Qt.TextSelectableByMouse)
         self.metaUserL.addWidget(label)
         self.metaUserW.show()
       else:
         link = False
         dataHierarchyItem = [i for group in dataHierarchyNode for i in dataHierarchyNode[group] if i['name']==key]
-        if isinstance(self.doc[key],str) and '\n' in self.doc[key]:     #if returns in value: format nicely
+        if (isinstance(self.doc[key],str) and '\n' in self.doc[key]) or key=='comment':
           labelW, labelL = widgetAndLayout('H', self.metaDetailsL, top='s', bottom='s')
           labelL.addWidget(QLabel(f'{key}: '), alignment=Qt.AlignTop) # type: ignore
           text = QTextEdit()
           text.setMarkdown(markdownStyler(self.doc[key]))
           bgColor = getColor(self.comm.backend, 'secondaryDark')
           fgColor = getColor(self.comm.backend, 'primaryText')
           text.setStyleSheet(f"QTextEdit {{ border: none; padding: 0px; background-color: {bgColor}; "\
                                 f"color: {fgColor} }}")
           text.document().setTextWidth(labelW.width())
+          self.rescaleTexts.append(text)
           height:int = text.document().size().toTuple()[1] # type: ignore[index]
           text.setFixedHeight(height)
           text.setReadOnly(True)
           labelL.addWidget(text, stretch=1) # type: ignore[call-arg]
         else:
           if len(dataHierarchyItem)==1 and 'list' in dataHierarchyItem[0]:
             if not isinstance(dataHierarchyItem[0]['list'], list):                #choice among docType
@@ -233,10 +236,24 @@
       docID (str): docID to which to link
     """
     logging.debug('used link on %s|%s',label,docID)
     self.comm.changeDetails.emit(docID)
     return
 
 
+  def resizeWidth(self, width:int) -> None:
+    """ called if details is resized by splitter at the parent widget
+    - resize all text-documents
+    """
+    if not self.rescaleTexts:
+      return
+    self.metaDetailsW.setFixedWidth(width)
+    for text in self.rescaleTexts:
+      text.document().setTextWidth(width)
+      height:int = text.document().size().toTuple()[1] #type: ignore[index]
+      text.setFixedHeight(height)
+    return
+
+
 class Command(Enum):
   """ Commands used in this file """
   SHOW             = 1
```

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/docTypes.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/docTypes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ widget that shows the table and the details of the items """
+from typing import Any
 from PySide6.QtCore import Slot                                # pylint: disable=no-name-in-module
 from PySide6.QtWidgets import QWidget, QSplitter, QVBoxLayout  # pylint: disable=no-name-in-module
 from .table import Table
 from .details import Details
 from ..guiCommunicate import Communicate
 
 class DocTypes(QWidget):
@@ -10,14 +11,15 @@
   def __init__(self, comm:Communicate):
     super().__init__()
     comm.changeTable.connect(self.changeTable)
     comm.changeDetails.connect(self.changeDetails)
     # GUI elements
     table = Table(comm)
     self.details = Details(comm)
+    self.details.resizeEvent = self.resizeWidget # type: ignore
     splitter = QSplitter()
     splitter.setHandleWidth(10)
     splitter.addWidget(table)
     splitter.addWidget(self.details)
     splitter.setContentsMargins(0,0,0,0)
     splitter.setSizes([1,1])
     mainL = QVBoxLayout()
@@ -49,7 +51,13 @@
 
     Args:
       docID (str): document ID
     """
     if docID!='':
       self.details.show()
     return
+
+
+  def resizeWidget(self, _:Any) -> None:
+    """ called if splitter resizes details-view  """
+    self.details.resizeWidth(self.details.width())
+    return
```

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/form.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/form.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,16 @@
     if self.doc['-type'][0] in self.db.dataHierarchy:
       dataHierarchyNode = self.db.dataHierarchy[self.doc['-type'][0]]['meta']
     else:
       dataHierarchyNode = defaultDataHierarchyNode
     keysDataHierarchy = [i['name'] for group in dataHierarchyNode for i in dataHierarchyNode[group]]
     for keyInDocNotHierarchy in set(self.doc.keys()).difference(keysDataHierarchy ):
       dataHierarchyNode['default'].append({'name':keyInDocNotHierarchy})
-    self.allKeys = [i['name'] for group in dataHierarchyNode for i in dataHierarchyNode[group]]
+    self.allKeys = {i['name'] for group in dataHierarchyNode for i in dataHierarchyNode[group]}
+    self.allKeys = self.allKeys.union(self.doc.keys())
 
     # create tabs or not: depending on the number of groups
     if '-tags' not in self.doc:
       self.doc['-tags'] = []
     self.tabW = QTabWidget() #has count=0 if not connected
     if len(dataHierarchyNode)>1:
       self.tabW.setParent(self)
@@ -245,18 +246,18 @@
 
   def autosave(self) -> None:
     """ Autosave comment to file """
     if self.comm.backend.configuration['GUI']['autosave'] == 'No':
       return
     content = {'-name': getattr(self, 'key_-name').text().strip()}
     for key in self.doc.keys():
-      if key[0] in self.skipKeys0 or key in self.skipKeys or not hasattr(self, f'key_{key}'):
-        continue
       if key in ['comment','content']:
         content[key] = getattr(self, f'textEdit_{key}').toPlainText().strip()
+      elif key[0] in self.skipKeys0 or key in self.skipKeys or not hasattr(self, f'key_{key}'):
+        continue
       elif isinstance(getattr(self, f'key_{key}'), QLineEdit):
         content[key] = getattr(self, f'key_{key}').text().strip()
       # skip QCombobox items since cannot be sure that next from has them and they are easy to recreate
     with open(Path.home()/'.pastaELN.temp', 'w', encoding='utf-8') as fTemp:
       fTemp.write(json.dumps(content))
     return
 
@@ -357,16 +358,17 @@
           othersList = [createDirName(str(i),'x0', 0) for i in others] #create names
           while createDirName(self.doc['-name'],'x0', 0) in othersList:
             if re.search(r"_\d+$", self.doc['-name']) is None:
               self.doc['-name'] += '_1'
             else:
               self.doc['-name'] = '_'.join(self.doc['-name'].split('_')[:-1])+'_'+str(int(self.doc['-name'].split('_')[-1])+1)
       # loop through all the subitems
-      for key, valueOld in self.doc.items():
-        if (key[0] in ['_', '-'] or key in ['image', 'metaVendor', 'metaUser']
+      for key in self.allKeys:
+        valueOld = self.doc.get(key, '')
+        if (key[0] in ['_', '-'] or key in ['image', 'metaVendor', 'metaUser']  #tags are already saved
             or not hasattr(self, f'key_{key}') and not hasattr(self, f'textEdit_{key}')):
           continue
         if key in ['comment','content']:
           text = getattr(self, f'textEdit_{key}').toPlainText().strip()
           if '_ids' not in self.doc or text:  #if group edit, text has to have text
             self.doc[key] = text
             if key == 'content' and '-branch' in self.doc:
```

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/project.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,14 +115,15 @@
     fgColor = getColor(self.comm.backend, 'primaryText')
     self.commentTE.setStyleSheet(f"border: none; padding: 0px; background-color: {bgColor}; color: {fgColor}")
     self.commentTE.setReadOnly(True)
     self.commentResize(None)
     commentL.addWidget(self.commentTE)
     return
 
+
   def commentResize(self, _:Any) -> None:
     """ called if comment is resized because widget initially/finally knows its size
     - comment widget is hard coded size it depends on the rendered size
     """
     if self.commentTE is None or self.infoWSA is None or self.infoW_ is None:
       return
     self.commentTE.document().setTextWidth(self.infoWSA.width())
@@ -163,32 +164,45 @@
       if node.is_root:         #Project header
         self.projHeader()
       else:
         rootItem.appendRow(self.iterateTree(node))
     # collapse / expand depending on stored value
     # by iterating each leaf, and converting item and index
     root = self.model.invisibleRootItem()
-    for iRow in range(root.rowCount()):
-      item = self.model.item(iRow,0)
-      data = item.data(role=Qt.UserRole+1)         # type: ignore[operator]
-      if data['hierStack'].split('/')[-1][0]=='x':
-        index = self.model.indexFromItem(item)
-        self.tree.setExpanded(index, data['gui'][1])
+    self.setExpandedState(root)
     if selectedIndex is not None:
       self.tree.selectionModel().select(selectedIndex, QItemSelectionModel.Select)
       self.tree.setCurrentIndex(selectedIndex)# Item(selectedItem)
     self.mainL.addWidget(self.tree)
     logging.debug('ProjectView elements at 4: %i',self.mainL.count())
     if len(nodeHier.children)>0 and self.btnAddSubfolder is not None:
       self.btnAddSubfolder.setVisible(False)
     self.tree.expanded.connect(lambda index: self.actionExpandCollapse(index, True))
     self.tree.collapsed.connect(lambda index: self.actionExpandCollapse(index, False))
     return
 
 
+  def setExpandedState(self, node:QStandardItem) -> None:
+    """ Recursive function to set the expanded state of nodes
+
+    Args:
+      node (QStandardItem): node to process
+    """
+    if self.model is None or self.tree is None:
+      return
+    for iRow in range(node.rowCount()):
+      item = node.child(iRow)
+      data = item.data(role=Qt.UserRole+1)         # type: ignore[operator]
+      if data['hierStack'].split('/')[-1][0]=='x':
+        index = self.model.indexFromItem(item)
+        self.tree.setExpanded(index, data['gui'][1])
+      self.setExpandedState(item)
+    return
+
+
   def actionExpandCollapse(self, index:QModelIndex, flag:bool) -> None:
     """ Action upon expansion or collapsing of folder (showing its children)
 
     Args:
       index (QModelIndex): index that send the signal
       flag (bool): true=expand=show-children, false=collapse=hide-children
     """
@@ -212,14 +226,15 @@
       self.comm.formDoc.emit(self.docProj)
       self.change(self.projID,'')
       #collect information and then change
       oldPath = self.comm.backend.basePath/self.docProj['-branch'][0]['path']
       if oldPath.is_dir():
         newPath = self.comm.backend.basePath/createDirName(self.docProj['-name'],'x0',0)
         oldPath.rename(newPath)
+      self.comm.changeSidebar.emit('redraw')
     elif command[0] is Command.DELETE:
       ret = QMessageBox.critical(self, 'Warning', 'Are you sure you want to delete project?', \
                       QMessageBox.StandardButton.No | QMessageBox.StandardButton.Yes,  # type: ignore[operator]
                       QMessageBox.StandardButton.No)
       if ret==QMessageBox.StandardButton.Yes:
         #delete database and rename folder
         doc = self.comm.backend.db.remove(self.projID)
```

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/projectGroup.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/projectGroup.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/projectLeafRenderer.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/projectLeafRenderer.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/projectTreeView.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/projectTreeView.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
   """ Custom tree view on data model """
   def __init__(self, parent:QWidget, comm:Communicate, model:QStandardItemModel):
     super().__init__(parent)
     self.comm = comm
     self.setModel(model)
     self.setHeaderHidden(True)
     self.setStyleSheet('QTreeView::branch {border-image: none;}')
+    self.setExpandsOnDoubleClick(False)
     self.setIndentation(40)
     self.renderer = ProjectLeafRenderer(self.comm)
     self.setItemDelegate(self.renderer)
     self.setDragDropMode(QAbstractItemView.InternalMove)
     self.doubleClicked.connect(self.tree2Clicked)
 
 
@@ -29,14 +30,16 @@
     """
     create context menu
 
     Args:
       p (QPoint): point of clicking
     """
     item = self.model().itemFromIndex(self.currentIndex())
+    if item is None:  #clicked outside any leaf
+      return
     folder = item.data()['hierStack'].split('/')[-1][0]=='x'
     context = QMenu(self)
     if folder:
       Action('Add child folder',                   self, [Command.ADD_CHILD],      context)
     Action('Add sibling folder',                   self, [Command.ADD_SIBLING],    context)
     Action('Delete item',                          self, [Command.DELETE],         context)
     context.addSeparator()
```

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/sidebar.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/sidebar.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/table.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         if self.docType in self.comm.backend.db.dataLabels:
           docLabel = self.comm.backend.db.dataLabels[self.docType]
       if self.projID:
         self.headline.setText(docLabel)
         self.showHidden.setText(f'Show/hide hidden {docLabel.lower()}')
       else:
         self.comm.changeSidebar.emit('')  #close the project in sidebar
-        self.headline.setText(f'All {docLabel}')
+        self.headline.setText(f'All {docLabel.lower()}')
         self.showHidden.setText(f'Show/hide all hidden {docLabel.lower()}')
       self.filterHeader = self.comm.backend.db.getColumnNames()[self.docType].split(',')
       self.filterHeader = [i[1:] if i[0]=='-'   else i for i in self.filterHeader]  #change -something to something
       self.filterHeader = [i[2:] if i[:2]=='#_' else i for i in self.filterHeader]  #change #_something to something
     self.headerW.show()
     nrows, ncols = len(self.data), len(self.filterHeader)
     model = QStandardItemModel(nrows, ncols)
@@ -331,15 +331,15 @@
             continue
           redraw = True
           oldDocType = doc['-type']
           if doc['-branch'][0]['path'].startswith('http'):
             path = Path(doc['-branch'][0]['path'])
           else:
             path = self.comm.backend.basePath/doc['-branch'][0]['path']
-          self.comm.backend.useExtractors(path, '', doc)
+          self.comm.backend.useExtractors(path, doc.get('shasum',''), doc)
           if doc['-type'][0] == oldDocType[0]:
             del doc['-branch']  #don't update
             self.comm.backend.db.updateDoc(doc, self.data[row]['id'])
           else:
             self.comm.backend.db.remove( self.data[row]['id'] )
             del doc['_id']
             del doc['_rev']
```

### Comparing `pasta_eln-2.5.0b8/pasta_eln/GUI/tableHeader.py` & `pasta_eln-2.5.1b1/pasta_eln/GUI/tableHeader.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/Resources/ExampleMeasurements/simple.png` & `pasta_eln-2.5.1b1/pasta_eln/Resources/ExampleMeasurements/simple.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/Resources/ExampleMeasurements/story.odt` & `pasta_eln-2.5.1b1/pasta_eln/Resources/ExampleMeasurements/story.odt`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/Resources/Icons/favicon64.ico` & `pasta_eln-2.5.1b1/pasta_eln/Resources/Icons/favicon64.ico`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/Resources/Icons/favicon64.png` & `pasta_eln-2.5.1b1/pasta_eln/Resources/Icons/favicon64.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/Resources/Icons/ols.png` & `pasta_eln-2.5.1b1/pasta_eln/Resources/Icons/ols.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/Resources/Icons/tib.png` & `pasta_eln-2.5.1b1/pasta_eln/Resources/Icons/tib.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/Resources/Icons/wikidata.png` & `pasta_eln-2.5.1b1/pasta_eln/Resources/Icons/wikidata.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/Resources/Icons/wikipedia.png` & `pasta_eln-2.5.1b1/pasta_eln/Resources/Icons/wikipedia.png`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/backend.py` & `pasta_eln-2.5.1b1/pasta_eln/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Python Backend: all operations with the filesystem are here """
 import json, sys, os, importlib, tempfile, logging, traceback
+from threading import Thread
 from pathlib import Path
 from typing import Any, Optional, Union
 from urllib import request
 from datetime import datetime, timezone
 from .mixin_cli import CLI_Mixin
 from .database import Database
 from .miscTools import upOut, createDirName, generic_hash, camelCase
@@ -115,30 +116,41 @@
       self.cwd     = self.basePath/doc['-branch'][0]['path']
     self.hierStack = doc['-branch'][0]['stack']+[doc['_id']]
     doc['childNum']= doc['-branch'][0]['child']
     # change content
     self.addData('-edit-', doc)
     # change folder-name in database of all children
     if doc['-type'][0][0]=='x' and self.cwd is not None:
-      items = self.db.getView(
-          'viewHierarchy/viewPaths',
-          startKey=f'{self.cwd.relative_to(self.basePath).as_posix()}/',
-      )
+      items = self.db.getView('viewHierarchy/viewPaths',
+                              startKey=f'{self.cwd.relative_to(self.basePath).as_posix()}/')
       for item in items:
-        oldPathparts = item['key'].split('/')
-        newPathParts = doc['-branch']['path'].split('/')
-        newPath = '/'.join(newPathParts+oldPathparts[len(newPathParts):]  )
-        # print(item['id']+'  old='+item['key']+'  branch='+str(item['value'][-1])+\
-        #      '  child='+str(item['value'][-3])+'  new='+newPath)
-        self.db.updateBranch(item['id'], item['value'][-1], item['value'][-3], path=newPath)
+        t = Thread(target=self.threadParallel, args=(item, doc))
+        t.start()
     self.cwd = self.basePath #reset to sensible before continuing
     self.hierStack = []
     return
 
 
+  def threadParallel(self, item:dict[str,Any], doc:dict[str,Any]) -> None:
+    """ internal function to process items and documents in parallel: rename folders on the disk
+
+    Args:
+      item (dict): item of current item to process
+      doc (dict):  parents documents
+    """
+    oldPathParts = item['key'].split('/')
+    newPathParts = doc['-branch']['path'].split('/')
+    newPath = '/'.join(newPathParts+oldPathParts[len(newPathParts):]  )
+    if newPath != item['key']:  # for-loop could also be implemented in parallel
+      # print(item['id']+'  old='+item['key']+'  branch='+str(item['value'][-1])+\
+      #      '  child='+str(item['value'][-3])+'  new='+newPath)
+      self.db.updateBranch(item['id'], item['value'][-1], item['value'][-3], path=newPath)
+    return
+
+
   def addData(self, docType:str, doc:dict[str,Any], hierStack:list[str]=[], localCopy:bool=False,
               forceNewImage:bool=False) -> str:
     """
     Save doc to database, also after edit
 
     Args:
         docType (string): docType to be stored, subtypes are / separated; or '-edit-'
```

### Comparing `pasta_eln-2.5.0b8/pasta_eln/cli.py` & `pasta_eln-2.5.1b1/pasta_eln/cli.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/database.py` & `pasta_eln-2.5.1b1/pasta_eln/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -457,25 +457,20 @@
     if docID[0]=='x' and path is not None:
       with open(self.basePath/path/'.id_pastaELN.json', 'w', encoding='utf-8') as fOut:
         fOut.write(json.dumps(self.getDoc(docID)))
       # update children's paths
       children = self.getView('viewHierarchy/viewHierarchy', startKey=' '.join(stackOld+[docID,'']))
       for line in children:
         docLine = self.db[line['id']]
-        flagNotChanged = True
         for branchLine in docLine['-branch']:
           if branchLine['path'] is not None and branchLine['path'].startswith(oldPath):
             branchLine['path'] = path+branchLine['path'][len(oldPath):]
-            flagNotChanged = False
           if stack is not None and '/'.join(branchLine['stack']).startswith('/'.join(stackOld)):
             branchLine['stack'] = stack+branchLine['stack'][len(stackOld):]
             branchLine['show']  = self.createShowFromStack(branchLine['stack'], branchLine['show'][-1])
-            flagNotChanged = False
-        if flagNotChanged:
-          print(f"**Unsure** Not updated{str(line)}")
         docLine.save()
         # update .json on disk
         for branchLine in docLine['-branch']:
           if line['id'][0]=='x'  and (self.basePath/branchLine['path']).is_dir():
             with open(self.basePath/branchLine['path']/'.id_pastaELN.json', 'w', encoding='utf-8') as fOut:
               fOut.write(json.dumps(docLine))
     return oldPath, path
```

### Comparing `pasta_eln-2.5.0b8/pasta_eln/dataverse/base_database_api.py` & `pasta_eln-2.5.1b1/pasta_eln/dataverse/base_database_api.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/dataverse/base_model.py` & `pasta_eln-2.5.1b1/pasta_eln/dataverse/base_model.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/dataverse/client.py` & `pasta_eln-2.5.1b1/pasta_eln/dataverse/client.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/dataverse/config_error.py` & `pasta_eln-2.5.1b1/pasta_eln/dataverse/config_error.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/dataverse/config_model.py` & `pasta_eln-2.5.1b1/pasta_eln/dataverse/config_model.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/dataverse/data_upload_task.py` & `pasta_eln-2.5.1b1/pasta_eln/dataverse/data_upload_task.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/dataverse/database_api.py` & `pasta_eln-2.5.1b1/pasta_eln/dataverse/database_api.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/dataverse/database_error.py` & `pasta_eln-2.5.1b1/pasta_eln/dataverse/database_error.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/dataverse/dataset-create-new-all-default-fields.json` & `pasta_eln-2.5.1b1/pasta_eln/dataverse/dataset-create-new-all-default-fields.json`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/dataverse/generic_task_object.py` & `pasta_eln-2.5.1b1/pasta_eln/dataverse/generic_task_object.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/dataverse/incorrect_parameter_error.py` & `pasta_eln-2.5.1b1/pasta_eln/dataverse/incorrect_parameter_error.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/dataverse/project_model.py` & `pasta_eln-2.5.1b1/pasta_eln/dataverse/project_model.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/dataverse/task_thread_extension.py` & `pasta_eln-2.5.1b1/pasta_eln/dataverse/task_thread_extension.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/dataverse/upload_model.py` & `pasta_eln-2.5.1b1/pasta_eln/dataverse/upload_model.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/dataverse/upload_queue_manager.py` & `pasta_eln-2.5.1b1/pasta_eln/dataverse/upload_queue_manager.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/dataverse/upload_status_values.py` & `pasta_eln-2.5.1b1/pasta_eln/dataverse/upload_status_values.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/dataverse/utils.py` & `pasta_eln-2.5.1b1/pasta_eln/dataverse/utils.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/fixedStringsJson.py` & `pasta_eln-2.5.1b1/pasta_eln/fixedStringsJson.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/gui.py` & `pasta_eln-2.5.1b1/pasta_eln/gui.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/guiCommunicate.py` & `pasta_eln-2.5.1b1/pasta_eln/guiCommunicate.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/guiStyle.py` & `pasta_eln-2.5.1b1/pasta_eln/guiStyle.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/handleDictionaries.py` & `pasta_eln-2.5.1b1/pasta_eln/handleDictionaries.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,18 @@
 
   Args:
     aDict (dict): dictionary to be translated
   """
   text = '<ul>'
   for key, value in aDict.items():
     if isinstance(value,str) and value.startswith('{') and value.endswith('}'):
-      value = json.loads(value.replace("'",'"'))
+      try:
+        value = json.loads(value.replace("'",'"'))
+      except:
+        pass
     if isinstance(value, dict):
       valueString = dict2ul(value)
     elif isinstance(value, list):
       valueString = ',&nbsp;&nbsp;&nbsp;'.join([str(i) for i in value])
     else:
       valueString = str(value)
     text += f'<li>{key}: {valueString}</li>\n'
```

### Comparing `pasta_eln-2.5.0b8/pasta_eln/inputOutput.py` & `pasta_eln-2.5.1b1/pasta_eln/inputOutput.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/installationTools.py` & `pasta_eln-2.5.1b1/pasta_eln/installationTools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-'''  Methods that check, repair, the local PASTA-ELN installation '''
+'''  Methods that check, repair, the local PASTA-ELN installation: no Qt-here '''
 import os, platform, sys, json, shutil, random, string, logging, uuid
 from typing import Optional, Any, Callable
 import urllib.request
 from pathlib import Path
 from cloudant.client import CouchDB
 
 from .backend import Backend
@@ -87,14 +87,29 @@
                             lpParameters=" ".join(cmdLine[1:]))
   procHandle = procInfo['hProcess']
   _ = win32event.WaitForSingleObject(procHandle, win32event.INFINITE)
   _   = win32process.GetExitCodeProcess(procHandle)
   return
 
 
+def checkForDotNetVersion() -> bool:
+  ''' check if .NET version 3.5 is installed (only on windows)
+  '''
+  import subprocess
+  command = ['reg','query','HKEY_LOCAL_MACHINE\\SOFTWARE\\Microsoft\\NET Framework Setup\\NDP','/s']
+  result = subprocess.run(command, stdout=subprocess.PIPE, check=True)
+  #### For reference: code to show all installed versions
+  # lines = [str(i).strip() for i in result.stdout.split(b'\n')]
+  # lines = [i.split()[3][:-3] for i in lines if 'Version' in i]
+  # versions = set(lines)
+  # count3_5 = len([i for i in versions if i.startswith('3.5.')])
+  # return count3_5>0
+  return b'Version    REG_SZ    3.5' in result.stdout
+
+
 def couchdb(command:str='test') -> str:
   '''
   test couchDB installation or (install it on Windows-only)
 
   Args:
     command (string): 'test' or 'install'
 
@@ -110,15 +125,15 @@
     except Exception:
       pass
     return '**ERROR**'
 
   elif command == 'install':
     if platform.system()=='Linux':
       return '**ERROR should not be called'
-    elif platform.system()=='Windows':
+    if platform.system()=='Windows':
       logging.info('CouchDB starting ...')
       url = 'https://couchdb.neighbourhood.ie/downloads/3.1.1/win/apache-couchdb-3.1.1.msi'
       path = Path.home()/'Downloads'/'apache-couchdb-3.1.1.msi'
       logging.info('Start download of couchdb')
       _, _ = urllib.request.urlretrieve(url, path)
       ## Old version with installer
       # cmd = ['cmd.exe','/K ',str(resultFilePath)]
```

### Comparing `pasta_eln-2.5.0b8/pasta_eln/miscTools.py` & `pasta_eln-2.5.1b1/pasta_eln/miscTools.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/mixin_cli.py` & `pasta_eln-2.5.1b1/pasta_eln/mixin_cli.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/printer.py` & `pasta_eln-2.5.1b1/pasta_eln/printer.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/serverActions.py` & `pasta_eln-2.5.1b1/pasta_eln/serverActions.py`

 * *Files 2% similar despite different names*

```diff
@@ -339,15 +339,15 @@
   """
   # get username and password
   if not location:
     location = 'remote' if input('Enter location: [r] remote; else local: ')=='r' else 'local'
   if location=='local':
     location = '127.0.0.1'
     if not userName:
-      userName = input('Enter username: ').strip()
+      userName = input('Enter local admin username: ').strip()
     if not password:
       password = input('Enter password: ').strip()
   elif location=='remote':
     try:
       myString = cred.get_password('pastaDB','admin')
       if myString is None:
         print("**ERROR Could not get credentials from keyring 2. Please create manually.")
@@ -439,23 +439,25 @@
   else:
     print('**ERROR: wrong location given.')
     return
   if not fileName:
     possFiles = [i for i in os.listdir('.') if i.startswith('couchDB') and i.endswith('.zip')]
     for idx, i in enumerate(possFiles):
       print(f'[{str(idx + 1)}] {i}')
-    fileName = input(f'Which file to use for restored? (1-{len(possFiles)}) ')
-    fileName = possFiles[int(fileName)-1]
+    fileChoice = input(f'Which file to use for restored? (1-{len(possFiles)}) ')
+    fileName = possFiles[int(fileChoice)-1] if fileChoice else possFiles[0]
   # use information
   authUser = requests.auth.HTTPBasicAuth(userName, password)
   with ZipFile(fileName, 'r', compression=ZIP_DEFLATED) as zipFile:
     files = zipFile.namelist()
     #first run through: create documents and design documents
     for fileI in files:
       fileParts = fileI.split('/')[1:]
+      if fileParts==['pastaELN.json']: #do not recreate file, it is only there for manual recovery
+        continue
       database = fileParts[0]
       docID = fileParts[1]
       if docID.endswith('_attach'):
         continue #Do in second loop
       #test if database is exists: create otherwise
       resp = requests.get(f'http://{location}:5984/{database}/_all_docs', headers=headers, auth=authUser, timeout=10)
       if resp.status_code != 200 and resp.json()['reason']=='Database does not exist.':
@@ -477,14 +479,16 @@
           if resp.ok:
             print('Saved document:', database, docID)
           else:
             print("**ERROR: could not save document:",resp.reason, database, docID, '\n', doc)
     #second run through: create attachments
     for fileI in files:
       fileParts = fileI.split('/')[1:]
+      if fileParts==['pastaELN.json']: #do not recreate file, it is only there for manual recovery
+        continue
       database = fileParts[0]
       docID = fileParts[1]
       if not docID.endswith('_attach'):
         continue #Did already in the first loop
       #test if attachment exists: create otherwise
       attachPath = f'{docID[:-7]}/{fileParts[-1]}'
       resp = requests.get(f'http://{location}:5984/{database}/{attachPath}', headers=headers, auth=authUser, timeout=10)
@@ -514,15 +518,15 @@
     if myString is None:
       print("**ERROR Could not get credentials from keyring 1. Please create manually.")
       print("import keyring as cred\nmyString = url+':'+adminUserName+':'+adminPassword\n#  url without http and port\ncred.set_password('pastaDB','admin',myString)")
       sys.exit(1)
     url, administrator, password = myString.split(':')
     print("URL and credentials successfully read from keyring")
   except Exception:
-    print("Could not get credentials from keyring.")
+    print("Could not get credentials for the remote server from keyring.")
     ## URL
     url = input('Enter the URL without http and without port: ')
     if len(url)<2:
       print('* No legit URL entered: exit')
       sys.exit(1)
     ## User-name, password
     administrator = input('Enter the administrator username: ')
```

### Comparing `pasta_eln-2.5.0b8/pasta_eln/utils.py` & `pasta_eln-2.5.1b1/pasta_eln/utils.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln/webclient/http_client.py` & `pasta_eln-2.5.1b1/pasta_eln/webclient/http_client.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/pasta_eln.egg-info/PKG-INFO` & `pasta_eln-2.5.1b1/pasta_eln.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasta_eln
-Version: 2.5.0b8
+Version: 2.5.1b1
 Summary: The favorite ELN for experimental scientists
 Home-page: https://pasta-eln.github.io/
 Author: The PASTA-ELN Team and Steffen Brinckmann
 Author-email: sbrinckm@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pasta_eln-2.5.0b8/pasta_eln.egg-info/SOURCES.txt` & `pasta_eln-2.5.1b1/pasta_eln.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/setup.cfg` & `pasta_eln-2.5.1b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/tests/test_01_3Projects.py` & `pasta_eln-2.5.1b1/tests/test_01_3Projects.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/tests/test_02_3Projects_ExportImport.py` & `pasta_eln-2.5.1b1/tests/test_02_3Projects_ExportImport.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/tests/test_50_importOthers.py` & `pasta_eln-2.5.1b1/tests/test_50_importOthers.py`

 * *Files identical despite different names*

### Comparing `pasta_eln-2.5.0b8/tests/test_99_3Projects.py` & `pasta_eln-2.5.1b1/tests/test_99_3Projects.py`

 * *Files identical despite different names*

