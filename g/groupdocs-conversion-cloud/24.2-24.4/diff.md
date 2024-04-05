# Comparing `tmp/groupdocs-conversion-cloud-24.2.tar.gz` & `tmp/groupdocs-conversion-cloud-24.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groupdocs-conversion-cloud-24.2.tar", last modified: Tue Feb 20 09:05:40 2024, max compression
+gzip compressed data, was "groupdocs-conversion-cloud-24.4.tar", last modified: Fri Apr  5 06:31:08 2024, max compression
```

## Comparing `groupdocs-conversion-cloud-24.2.tar` & `groupdocs-conversion-cloud-24.4.tar`

### file list

```diff
@@ -1,215 +1,218 @@
-drwxrwxrwx   0        0        0        0 2024-02-20 09:05:40.534029 groupdocs-conversion-cloud-24.2/
--rw-rw-rw-   0        0        0     1105 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/LICENSE
--rw-rw-rw-   0        0        0     3147 2024-02-20 09:05:40.533028 groupdocs-conversion-cloud-24.2/PKG-INFO
--rw-rw-rw-   0        0        0     2184 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/README.md
-drwxrwxrwx   0        0        0        0 2024-02-20 09:05:40.008015 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/
--rw-rw-rw-   0        0        0    15692 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/__init__.py
--rw-rw-rw-   0        0        0    26255 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/api_client.py
--rw-rw-rw-   0        0        0     2674 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/api_exception.py
-drwxrwxrwx   0        0        0        0 2024-02-20 09:05:40.034028 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/apis/
--rw-rw-rw-   0        0        0      469 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/apis/__init__.py
--rw-rw-rw-   0        0        0    20840 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/apis/convert_api.py
--rw-rw-rw-   0        0        0    38676 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/apis/file_api.py
--rw-rw-rw-   0        0        0    36286 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/apis/folder_api.py
--rw-rw-rw-   0        0        0    16416 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/apis/info_api.py
--rw-rw-rw-   0        0        0     9724 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/apis/license_api.py
--rw-rw-rw-   0        0        0    26598 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/apis/storage_api.py
--rw-rw-rw-   0        0        0     3307 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/auth.py
--rw-rw-rw-   0        0        0     7681 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/configuration.py
-drwxrwxrwx   0        0        0        0 2024-02-20 09:05:40.432026 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/
--rw-rw-rw-   0        0        0    14313 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/__init__.py
--rw-rw-rw-   0        0        0     6579 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/api_error.py
--rw-rw-rw-   0        0        0     4674 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/api_error_response.py
--rw-rw-rw-   0        0        0     3735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/bmp_convert_options.py
--rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/bmp_load_options.py
--rw-rw-rw-   0        0        0     6222 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/cad_load_options.py
--rw-rw-rw-   0        0        0     5129 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/consumption_result.py
--rw-rw-rw-   0        0        0     6987 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/convert_options.py
--rw-rw-rw-   0        0        0     9847 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/convert_settings.py
--rw-rw-rw-   0        0        0     9814 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/csv_load_options.py
--rw-rw-rw-   0        0        0     3735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/dcm_convert_options.py
--rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/dcm_load_options.py
--rw-rw-rw-   0        0        0     3707 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/dgn_load_options.py
--rw-rw-rw-   0        0        0     4660 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/diagram_load_options.py
--rw-rw-rw-   0        0        0     5187 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/disc_usage.py
--rw-rw-rw-   0        0        0     3741 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/djvu_convert_options.py
--rw-rw-rw-   0        0        0     3735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/dng_convert_options.py
--rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/dng_load_options.py
--rw-rw-rw-   0        0        0     3753 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/doc_convert_options.py
--rw-rw-rw-   0        0        0     3729 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/doc_load_options.py
--rw-rw-rw-   0        0        0     3759 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/docm_convert_options.py
--rw-rw-rw-   0        0        0     3735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/docm_load_options.py
--rw-rw-rw-   0        0        0    16808 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/document_metadata.py
--rw-rw-rw-   0        0        0     3759 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/docx_convert_options.py
--rw-rw-rw-   0        0        0     3735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/docx_load_options.py
--rw-rw-rw-   0        0        0     3753 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/dot_convert_options.py
--rw-rw-rw-   0        0        0     3729 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/dot_load_options.py
--rw-rw-rw-   0        0        0     3759 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/dotm_convert_options.py
--rw-rw-rw-   0        0        0     3735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/dotm_load_options.py
--rw-rw-rw-   0        0        0     3759 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/dotx_convert_options.py
--rw-rw-rw-   0        0        0     3735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/dotx_load_options.py
--rw-rw-rw-   0        0        0     3707 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/dwf_load_options.py
--rw-rw-rw-   0        0        0     3707 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/dwg_load_options.py
--rw-rw-rw-   0        0        0     3707 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/dxf_load_options.py
--rw-rw-rw-   0        0        0     6730 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/e_book_convert_options.py
--rw-rw-rw-   0        0        0    15696 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/email_load_options.py
--rw-rw-rw-   0        0        0     3735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/emf_convert_options.py
--rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/emf_load_options.py
--rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/eml_load_options.py
--rw-rw-rw-   0        0        0     3717 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/emlx_load_options.py
--rw-rw-rw-   0        0        0     6291 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/error.py
--rw-rw-rw-   0        0        0     4905 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/error_details.py
--rw-rw-rw-   0        0        0     5457 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/field_label.py
--rw-rw-rw-   0        0        0     5413 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/file_version.py
--rw-rw-rw-   0        0        0     4151 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/file_versions.py
--rw-rw-rw-   0        0        0     4171 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/files_list.py
--rw-rw-rw-   0        0        0     4884 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/files_upload_result.py
--rw-rw-rw-   0        0        0     3735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/gif_convert_options.py
--rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/gif_load_options.py
--rw-rw-rw-   0        0        0     3735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ico_convert_options.py
--rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ico_load_options.py
--rw-rw-rw-   0        0        0     3707 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ifc_load_options.py
--rw-rw-rw-   0        0        0     3707 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/igs_load_options.py
--rw-rw-rw-   0        0        0    14501 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/image_convert_options.py
--rw-rw-rw-   0        0        0     4672 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/image_load_options.py
--rw-rw-rw-   0        0        0     3731 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/j2c_convert_options.py
--rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/j2c_load_options.py
--rw-rw-rw-   0        0        0     3731 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/j2k_convert_options.py
--rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/j2k_load_options.py
--rw-rw-rw-   0        0        0     3731 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/jp2_convert_options.py
--rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/jp2_load_options.py
--rw-rw-rw-   0        0        0     3737 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/jpeg_convert_options.py
--rw-rw-rw-   0        0        0     3717 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/jpeg_load_options.py
--rw-rw-rw-   0        0        0     3731 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/jpf_convert_options.py
--rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/jpf_load_options.py
--rw-rw-rw-   0        0        0     4728 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/jpg_convert_options.py
--rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/jpg_load_options.py
--rw-rw-rw-   0        0        0     3731 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/jpm_convert_options.py
--rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/jpm_load_options.py
--rw-rw-rw-   0        0        0     3731 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/jpx_convert_options.py
--rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/jpx_load_options.py
--rw-rw-rw-   0        0        0     4418 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/license_info.py
--rw-rw-rw-   0        0        0     4752 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/load_options.py
--rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/mht_load_options.py
--rw-rw-rw-   0        0        0     3735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/mobi_load_options.py
--rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/msg_load_options.py
--rw-rw-rw-   0        0        0     5178 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/object_exist.py
--rw-rw-rw-   0        0        0     3735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/odg_convert_options.py
--rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/odg_load_options.py
--rw-rw-rw-   0        0        0     3749 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/odp_convert_options.py
--rw-rw-rw-   0        0        0     3725 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/odp_load_options.py
--rw-rw-rw-   0        0        0     3747 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ods_convert_options.py
--rw-rw-rw-   0        0        0     3723 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ods_load_options.py
--rw-rw-rw-   0        0        0     3753 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/odt_convert_options.py
--rw-rw-rw-   0        0        0     3729 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/odt_load_options.py
--rw-rw-rw-   0        0        0     6360 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/one_load_options.py
--rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ost_load_options.py
--rw-rw-rw-   0        0        0     3749 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/otp_convert_options.py
--rw-rw-rw-   0        0        0     3725 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/otp_load_options.py
--rw-rw-rw-   0        0        0     3747 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ots_convert_options.py
--rw-rw-rw-   0        0        0     3723 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ots_load_options.py
--rw-rw-rw-   0        0        0     3753 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ott_convert_options.py
--rw-rw-rw-   0        0        0     3729 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ott_load_options.py
--rw-rw-rw-   0        0        0    40157 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/pdf_convert_options.py
--rw-rw-rw-   0        0        0     7811 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/pdf_load_options.py
--rw-rw-rw-   0        0        0     3747 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/pdl_convert_options.py
--rw-rw-rw-   0        0        0     5352 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/personal_storage_load_options.py
--rw-rw-rw-   0        0        0     3707 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/plt_load_options.py
--rw-rw-rw-   0        0        0     3735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/png_convert_options.py
--rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/png_load_options.py
--rw-rw-rw-   0        0        0     3755 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/potm_convert_options.py
--rw-rw-rw-   0        0        0     3731 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/potm_load_options.py
--rw-rw-rw-   0        0        0     3755 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/potx_convert_options.py
--rw-rw-rw-   0        0        0     3731 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/potx_load_options.py
--rw-rw-rw-   0        0        0     3749 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/pps_convert_options.py
--rw-rw-rw-   0        0        0     3725 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/pps_load_options.py
--rw-rw-rw-   0        0        0     3755 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ppsm_convert_options.py
--rw-rw-rw-   0        0        0     3731 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ppsm_load_options.py
--rw-rw-rw-   0        0        0     3755 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ppsx_convert_options.py
--rw-rw-rw-   0        0        0     3731 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ppsx_load_options.py
--rw-rw-rw-   0        0        0     3749 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ppt_convert_options.py
--rw-rw-rw-   0        0        0     3725 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ppt_load_options.py
--rw-rw-rw-   0        0        0     3755 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/pptm_convert_options.py
--rw-rw-rw-   0        0        0     3731 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/pptm_load_options.py
--rw-rw-rw-   0        0        0     3755 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/pptx_convert_options.py
--rw-rw-rw-   0        0        0     3731 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/pptx_load_options.py
--rw-rw-rw-   0        0        0     5877 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/presentation_convert_options.py
--rw-rw-rw-   0        0        0     8455 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/presentation_load_options.py
--rw-rw-rw-   0        0        0     9565 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/psd_convert_options.py
--rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/psd_load_options.py
--rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/pst_load_options.py
--rw-rw-rw-   0        0        0     5321 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/rtf_convert_options.py
--rw-rw-rw-   0        0        0     6360 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/spreadsheet_convert_options.py
--rw-rw-rw-   0        0        0    13028 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/spreadsheet_load_options.py
--rw-rw-rw-   0        0        0     3707 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/stl_load_options.py
--rw-rw-rw-   0        0        0     4276 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/storage_exist.py
--rw-rw-rw-   0        0        0     7173 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/storage_file.py
--rw-rw-rw-   0        0        0     6214 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/stored_converted_result.py
--rw-rw-rw-   0        0        0     5180 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/supported_format.py
--rw-rw-rw-   0        0        0     3733 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/tif_convert_options.py
--rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/tif_load_options.py
--rw-rw-rw-   0        0        0     4994 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/tiff_convert_options.py
--rw-rw-rw-   0        0        0     3717 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/tiff_load_options.py
--rw-rw-rw-   0        0        0     3747 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/tsv_convert_options.py
--rw-rw-rw-   0        0        0     3723 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/tsv_load_options.py
--rw-rw-rw-   0        0        0     3725 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/txt_convert_options.py
--rw-rw-rw-   0        0        0     9842 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/txt_load_options.py
--rw-rw-rw-   0        0        0     3715 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/vdw_load_options.py
--rw-rw-rw-   0        0        0     3715 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/vdx_load_options.py
--rw-rw-rw-   0        0        0     3715 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/vsd_load_options.py
--rw-rw-rw-   0        0        0     3721 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/vsdm_load_options.py
--rw-rw-rw-   0        0        0     3721 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/vsdx_load_options.py
--rw-rw-rw-   0        0        0     3715 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/vss_load_options.py
--rw-rw-rw-   0        0        0     3721 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/vssm_load_options.py
--rw-rw-rw-   0        0        0     3721 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/vssx_load_options.py
--rw-rw-rw-   0        0        0     3715 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/vst_load_options.py
--rw-rw-rw-   0        0        0     3721 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/vstm_load_options.py
--rw-rw-rw-   0        0        0     3721 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/vstx_load_options.py
--rw-rw-rw-   0        0        0     3715 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/vsx_load_options.py
--rw-rw-rw-   0        0        0     3715 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/vtx_load_options.py
--rw-rw-rw-   0        0        0    16187 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/watermark_options.py
--rw-rw-rw-   0        0        0     7852 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/web_convert_options.py
--rw-rw-rw-   0        0        0     4810 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/web_load_options.py
--rw-rw-rw-   0        0        0     4675 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/webp_convert_options.py
--rw-rw-rw-   0        0        0     3717 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/webp_load_options.py
--rw-rw-rw-   0        0        0     3735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/wmf_convert_options.py
--rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/wmf_load_options.py
--rw-rw-rw-   0        0        0    12939 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/word_processing_convert_options.py
--rw-rw-rw-   0        0        0    15011 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/word_processing_load_options.py
--rw-rw-rw-   0        0        0     3771 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xls2003_convert_options.py
--rw-rw-rw-   0        0        0     3747 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xls2003_load_options.py
--rw-rw-rw-   0        0        0     3747 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xls_convert_options.py
--rw-rw-rw-   0        0        0     3723 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xls_load_options.py
--rw-rw-rw-   0        0        0     3753 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xlsb_convert_options.py
--rw-rw-rw-   0        0        0     3729 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xlsb_load_options.py
--rw-rw-rw-   0        0        0     3753 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xlsm_convert_options.py
--rw-rw-rw-   0        0        0     3729 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xlsm_load_options.py
--rw-rw-rw-   0        0        0     3753 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xlsx_convert_options.py
--rw-rw-rw-   0        0        0     3729 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xlsx_load_options.py
--rw-rw-rw-   0        0        0     3753 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xltm_convert_options.py
--rw-rw-rw-   0        0        0     3729 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xltm_load_options.py
--rw-rw-rw-   0        0        0     3753 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xltx_convert_options.py
--rw-rw-rw-   0        0        0     3729 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xltx_load_options.py
--rw-rw-rw-   0        0        0     4763 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xml_load_options.py
--rw-rw-rw-   0        0        0    13739 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/rest.py
-drwxrwxrwx   0        0        0        0 2024-02-20 09:05:40.532061 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud.egg-info/
--rw-rw-rw-   0        0        0     3147 2024-02-20 09:05:39.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10758 2024-02-20 09:05:39.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-20 09:05:39.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-02-20 09:05:39.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2024-02-20 09:05:39.000000 groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-20 09:05:40.534029 groupdocs-conversion-cloud-24.2/setup.cfg
--rw-rw-rw-   0        0        0     1699 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-20 09:05:40.509037 groupdocs-conversion-cloud-24.2/test/
--rw-rw-rw-   0        0        0        0 2024-02-20 09:04:58.000000 groupdocs-conversion-cloud-24.2/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-20 09:05:40.531029 groupdocs-conversion-cloud-24.2/test/apis/
--rw-rw-rw-   0        0        0        0 2024-02-20 09:04:58.000000 groupdocs-conversion-cloud-24.2/test/apis/__init__.py
--rw-rw-rw-   0        0        0     3156 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/test/apis/test_auth_api.py
--rw-rw-rw-   0        0        0     3956 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/test/apis/test_convert_api.py
--rw-rw-rw-   0        0        0     3802 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/test/apis/test_file_api.py
--rw-rw-rw-   0        0        0     3150 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/test/apis/test_folder_api.py
--rw-rw-rw-   0        0        0     2972 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/test/apis/test_info_api.py
--rw-rw-rw-   0        0        0     2735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/test/apis/test_storage_api.py
--rw-rw-rw-   0        0        0     4794 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/test/test_context.py
--rw-rw-rw-   0        0        0     2445 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/test/test_file.py
--rw-rw-rw-   0        0        0     1680 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.2/test/test_settings.py
+drwxrwxrwx   0        0        0        0 2024-04-05 06:31:08.977781 groupdocs-conversion-cloud-24.4/
+-rw-rw-rw-   0        0        0     1105 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/LICENSE
+-rw-rw-rw-   0        0        0     3147 2024-04-05 06:31:08.976781 groupdocs-conversion-cloud-24.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2184 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 06:31:08.234782 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/
+-rw-rw-rw-   0        0        0    15931 2024-04-05 06:30:33.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/__init__.py
+-rw-rw-rw-   0        0        0    26255 2024-04-05 06:30:33.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/api_client.py
+-rw-rw-rw-   0        0        0     2674 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/api_exception.py
+drwxrwxrwx   0        0        0        0 2024-04-05 06:31:08.252780 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/apis/
+-rw-rw-rw-   0        0        0      469 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/apis/__init__.py
+-rw-rw-rw-   0        0        0    20840 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/apis/convert_api.py
+-rw-rw-rw-   0        0        0    38676 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/apis/file_api.py
+-rw-rw-rw-   0        0        0    36286 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/apis/folder_api.py
+-rw-rw-rw-   0        0        0    16416 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/apis/info_api.py
+-rw-rw-rw-   0        0        0     9724 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/apis/license_api.py
+-rw-rw-rw-   0        0        0    26598 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/apis/storage_api.py
+-rw-rw-rw-   0        0        0     3307 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/auth.py
+-rw-rw-rw-   0        0        0     7681 2024-04-05 06:30:33.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/configuration.py
+drwxrwxrwx   0        0        0        0 2024-04-05 06:31:08.944780 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/
+-rw-rw-rw-   0        0        0    14552 2024-04-05 06:30:33.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/__init__.py
+-rw-rw-rw-   0        0        0     6579 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/api_error.py
+-rw-rw-rw-   0        0        0     4674 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/api_error_response.py
+-rw-rw-rw-   0        0        0     3735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/bmp_convert_options.py
+-rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/bmp_load_options.py
+-rw-rw-rw-   0        0        0     6766 2024-04-05 06:30:33.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/cad_load_options.py
+-rw-rw-rw-   0        0        0     3707 2024-04-05 06:30:33.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/cf2_load_options.py
+-rw-rw-rw-   0        0        0     5129 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/consumption_result.py
+-rw-rw-rw-   0        0        0     6987 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/convert_options.py
+-rw-rw-rw-   0        0        0     9847 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/convert_settings.py
+-rw-rw-rw-   0        0        0     9814 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/csv_load_options.py
+-rw-rw-rw-   0        0        0     3735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dcm_convert_options.py
+-rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dcm_load_options.py
+-rw-rw-rw-   0        0        0     3707 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dgn_load_options.py
+-rw-rw-rw-   0        0        0     4660 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/diagram_load_options.py
+-rw-rw-rw-   0        0        0     5187 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/disc_usage.py
+-rw-rw-rw-   0        0        0     3741 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/djvu_convert_options.py
+-rw-rw-rw-   0        0        0     3735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dng_convert_options.py
+-rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dng_load_options.py
+-rw-rw-rw-   0        0        0     3753 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/doc_convert_options.py
+-rw-rw-rw-   0        0        0     3729 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/doc_load_options.py
+-rw-rw-rw-   0        0        0     3759 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/docm_convert_options.py
+-rw-rw-rw-   0        0        0     3735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/docm_load_options.py
+-rw-rw-rw-   0        0        0    16808 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/document_metadata.py
+-rw-rw-rw-   0        0        0     3759 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/docx_convert_options.py
+-rw-rw-rw-   0        0        0     3735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/docx_load_options.py
+-rw-rw-rw-   0        0        0     3753 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dot_convert_options.py
+-rw-rw-rw-   0        0        0     3729 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dot_load_options.py
+-rw-rw-rw-   0        0        0     3759 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dotm_convert_options.py
+-rw-rw-rw-   0        0        0     3735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dotm_load_options.py
+-rw-rw-rw-   0        0        0     3759 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dotx_convert_options.py
+-rw-rw-rw-   0        0        0     3735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dotx_load_options.py
+-rw-rw-rw-   0        0        0     3707 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dwf_load_options.py
+-rw-rw-rw-   0        0        0     3713 2024-04-05 06:30:33.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dwfx_load_options.py
+-rw-rw-rw-   0        0        0     3707 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dwg_load_options.py
+-rw-rw-rw-   0        0        0     3707 2024-04-05 06:30:33.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dwt_load_options.py
+-rw-rw-rw-   0        0        0     3707 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dxf_load_options.py
+-rw-rw-rw-   0        0        0     6730 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/e_book_convert_options.py
+-rw-rw-rw-   0        0        0    15696 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/email_load_options.py
+-rw-rw-rw-   0        0        0     3735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/emf_convert_options.py
+-rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/emf_load_options.py
+-rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/eml_load_options.py
+-rw-rw-rw-   0        0        0     3717 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/emlx_load_options.py
+-rw-rw-rw-   0        0        0     6291 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/error.py
+-rw-rw-rw-   0        0        0     4905 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/error_details.py
+-rw-rw-rw-   0        0        0     5457 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/field_label.py
+-rw-rw-rw-   0        0        0     5413 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/file_version.py
+-rw-rw-rw-   0        0        0     4151 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/file_versions.py
+-rw-rw-rw-   0        0        0     4171 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/files_list.py
+-rw-rw-rw-   0        0        0     4884 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/files_upload_result.py
+-rw-rw-rw-   0        0        0     3735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/gif_convert_options.py
+-rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/gif_load_options.py
+-rw-rw-rw-   0        0        0     3735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ico_convert_options.py
+-rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ico_load_options.py
+-rw-rw-rw-   0        0        0     3707 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ifc_load_options.py
+-rw-rw-rw-   0        0        0     3707 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/igs_load_options.py
+-rw-rw-rw-   0        0        0    14501 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/image_convert_options.py
+-rw-rw-rw-   0        0        0     4672 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/image_load_options.py
+-rw-rw-rw-   0        0        0     3731 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/j2c_convert_options.py
+-rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/j2c_load_options.py
+-rw-rw-rw-   0        0        0     3731 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/j2k_convert_options.py
+-rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/j2k_load_options.py
+-rw-rw-rw-   0        0        0     3731 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/jp2_convert_options.py
+-rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/jp2_load_options.py
+-rw-rw-rw-   0        0        0     3737 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/jpeg_convert_options.py
+-rw-rw-rw-   0        0        0     3717 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/jpeg_load_options.py
+-rw-rw-rw-   0        0        0     3731 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/jpf_convert_options.py
+-rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/jpf_load_options.py
+-rw-rw-rw-   0        0        0     4728 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/jpg_convert_options.py
+-rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/jpg_load_options.py
+-rw-rw-rw-   0        0        0     3731 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/jpm_convert_options.py
+-rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/jpm_load_options.py
+-rw-rw-rw-   0        0        0     3731 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/jpx_convert_options.py
+-rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/jpx_load_options.py
+-rw-rw-rw-   0        0        0     4418 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/license_info.py
+-rw-rw-rw-   0        0        0     4752 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/load_options.py
+-rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/mht_load_options.py
+-rw-rw-rw-   0        0        0     3735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/mobi_load_options.py
+-rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/msg_load_options.py
+-rw-rw-rw-   0        0        0     5178 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/object_exist.py
+-rw-rw-rw-   0        0        0     3735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/odg_convert_options.py
+-rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/odg_load_options.py
+-rw-rw-rw-   0        0        0     3749 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/odp_convert_options.py
+-rw-rw-rw-   0        0        0     3725 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/odp_load_options.py
+-rw-rw-rw-   0        0        0     3747 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ods_convert_options.py
+-rw-rw-rw-   0        0        0     3723 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ods_load_options.py
+-rw-rw-rw-   0        0        0     3753 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/odt_convert_options.py
+-rw-rw-rw-   0        0        0     3729 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/odt_load_options.py
+-rw-rw-rw-   0        0        0     6360 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/one_load_options.py
+-rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ost_load_options.py
+-rw-rw-rw-   0        0        0     3749 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/otp_convert_options.py
+-rw-rw-rw-   0        0        0     3725 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/otp_load_options.py
+-rw-rw-rw-   0        0        0     3747 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ots_convert_options.py
+-rw-rw-rw-   0        0        0     3723 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ots_load_options.py
+-rw-rw-rw-   0        0        0     3753 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ott_convert_options.py
+-rw-rw-rw-   0        0        0     3729 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ott_load_options.py
+-rw-rw-rw-   0        0        0    40157 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/pdf_convert_options.py
+-rw-rw-rw-   0        0        0     7811 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/pdf_load_options.py
+-rw-rw-rw-   0        0        0     3747 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/pdl_convert_options.py
+-rw-rw-rw-   0        0        0     5352 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/personal_storage_load_options.py
+-rw-rw-rw-   0        0        0     3707 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/plt_load_options.py
+-rw-rw-rw-   0        0        0     3735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/png_convert_options.py
+-rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/png_load_options.py
+-rw-rw-rw-   0        0        0     3755 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/potm_convert_options.py
+-rw-rw-rw-   0        0        0     3731 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/potm_load_options.py
+-rw-rw-rw-   0        0        0     3755 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/potx_convert_options.py
+-rw-rw-rw-   0        0        0     3731 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/potx_load_options.py
+-rw-rw-rw-   0        0        0     3749 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/pps_convert_options.py
+-rw-rw-rw-   0        0        0     3725 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/pps_load_options.py
+-rw-rw-rw-   0        0        0     3755 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ppsm_convert_options.py
+-rw-rw-rw-   0        0        0     3731 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ppsm_load_options.py
+-rw-rw-rw-   0        0        0     3755 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ppsx_convert_options.py
+-rw-rw-rw-   0        0        0     3731 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ppsx_load_options.py
+-rw-rw-rw-   0        0        0     3749 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ppt_convert_options.py
+-rw-rw-rw-   0        0        0     3725 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ppt_load_options.py
+-rw-rw-rw-   0        0        0     3755 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/pptm_convert_options.py
+-rw-rw-rw-   0        0        0     3731 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/pptm_load_options.py
+-rw-rw-rw-   0        0        0     3755 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/pptx_convert_options.py
+-rw-rw-rw-   0        0        0     3731 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/pptx_load_options.py
+-rw-rw-rw-   0        0        0     5877 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/presentation_convert_options.py
+-rw-rw-rw-   0        0        0     8455 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/presentation_load_options.py
+-rw-rw-rw-   0        0        0     9565 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/psd_convert_options.py
+-rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/psd_load_options.py
+-rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/pst_load_options.py
+-rw-rw-rw-   0        0        0     5321 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/rtf_convert_options.py
+-rw-rw-rw-   0        0        0     6360 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/spreadsheet_convert_options.py
+-rw-rw-rw-   0        0        0    13028 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/spreadsheet_load_options.py
+-rw-rw-rw-   0        0        0     3707 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/stl_load_options.py
+-rw-rw-rw-   0        0        0     4276 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/storage_exist.py
+-rw-rw-rw-   0        0        0     7173 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/storage_file.py
+-rw-rw-rw-   0        0        0     6214 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/stored_converted_result.py
+-rw-rw-rw-   0        0        0     5180 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/supported_format.py
+-rw-rw-rw-   0        0        0     3733 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/tif_convert_options.py
+-rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/tif_load_options.py
+-rw-rw-rw-   0        0        0     4994 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/tiff_convert_options.py
+-rw-rw-rw-   0        0        0     3717 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/tiff_load_options.py
+-rw-rw-rw-   0        0        0     3747 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/tsv_convert_options.py
+-rw-rw-rw-   0        0        0     3723 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/tsv_load_options.py
+-rw-rw-rw-   0        0        0     3725 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/txt_convert_options.py
+-rw-rw-rw-   0        0        0     9842 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/txt_load_options.py
+-rw-rw-rw-   0        0        0     3715 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/vdw_load_options.py
+-rw-rw-rw-   0        0        0     3715 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/vdx_load_options.py
+-rw-rw-rw-   0        0        0     3715 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/vsd_load_options.py
+-rw-rw-rw-   0        0        0     3721 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/vsdm_load_options.py
+-rw-rw-rw-   0        0        0     3721 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/vsdx_load_options.py
+-rw-rw-rw-   0        0        0     3715 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/vss_load_options.py
+-rw-rw-rw-   0        0        0     3721 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/vssm_load_options.py
+-rw-rw-rw-   0        0        0     3721 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/vssx_load_options.py
+-rw-rw-rw-   0        0        0     3715 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/vst_load_options.py
+-rw-rw-rw-   0        0        0     3721 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/vstm_load_options.py
+-rw-rw-rw-   0        0        0     3721 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/vstx_load_options.py
+-rw-rw-rw-   0        0        0     3715 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/vsx_load_options.py
+-rw-rw-rw-   0        0        0     3715 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/vtx_load_options.py
+-rw-rw-rw-   0        0        0    16187 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/watermark_options.py
+-rw-rw-rw-   0        0        0     7852 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/web_convert_options.py
+-rw-rw-rw-   0        0        0     4810 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/web_load_options.py
+-rw-rw-rw-   0        0        0     4675 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/webp_convert_options.py
+-rw-rw-rw-   0        0        0     3717 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/webp_load_options.py
+-rw-rw-rw-   0        0        0     3735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/wmf_convert_options.py
+-rw-rw-rw-   0        0        0     3711 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/wmf_load_options.py
+-rw-rw-rw-   0        0        0    12939 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/word_processing_convert_options.py
+-rw-rw-rw-   0        0        0    15011 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/word_processing_load_options.py
+-rw-rw-rw-   0        0        0     3771 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xls2003_convert_options.py
+-rw-rw-rw-   0        0        0     3747 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xls2003_load_options.py
+-rw-rw-rw-   0        0        0     3747 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xls_convert_options.py
+-rw-rw-rw-   0        0        0     3723 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xls_load_options.py
+-rw-rw-rw-   0        0        0     3753 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xlsb_convert_options.py
+-rw-rw-rw-   0        0        0     3729 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xlsb_load_options.py
+-rw-rw-rw-   0        0        0     3753 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xlsm_convert_options.py
+-rw-rw-rw-   0        0        0     3729 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xlsm_load_options.py
+-rw-rw-rw-   0        0        0     3753 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xlsx_convert_options.py
+-rw-rw-rw-   0        0        0     3729 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xlsx_load_options.py
+-rw-rw-rw-   0        0        0     3753 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xltm_convert_options.py
+-rw-rw-rw-   0        0        0     3729 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xltm_load_options.py
+-rw-rw-rw-   0        0        0     3753 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xltx_convert_options.py
+-rw-rw-rw-   0        0        0     3729 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xltx_load_options.py
+-rw-rw-rw-   0        0        0     4763 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xml_load_options.py
+-rw-rw-rw-   0        0        0    13739 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/rest.py
+drwxrwxrwx   0        0        0        0 2024-04-05 06:31:08.975788 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud.egg-info/
+-rw-rw-rw-   0        0        0     3147 2024-04-05 06:31:07.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10921 2024-04-05 06:31:07.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 06:31:07.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-05 06:31:07.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2024-04-05 06:31:07.000000 groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 06:31:08.978780 groupdocs-conversion-cloud-24.4/setup.cfg
+-rw-rw-rw-   0        0        0     1699 2024-04-05 06:30:33.000000 groupdocs-conversion-cloud-24.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 06:31:08.951780 groupdocs-conversion-cloud-24.4/test/
+-rw-rw-rw-   0        0        0        0 2024-04-05 06:30:35.000000 groupdocs-conversion-cloud-24.4/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 06:31:08.973784 groupdocs-conversion-cloud-24.4/test/apis/
+-rw-rw-rw-   0        0        0        0 2024-04-05 06:30:35.000000 groupdocs-conversion-cloud-24.4/test/apis/__init__.py
+-rw-rw-rw-   0        0        0     3156 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/test/apis/test_auth_api.py
+-rw-rw-rw-   0        0        0     3956 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/test/apis/test_convert_api.py
+-rw-rw-rw-   0        0        0     3802 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/test/apis/test_file_api.py
+-rw-rw-rw-   0        0        0     3150 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/test/apis/test_folder_api.py
+-rw-rw-rw-   0        0        0     2972 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/test/apis/test_info_api.py
+-rw-rw-rw-   0        0        0     2735 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/test/apis/test_storage_api.py
+-rw-rw-rw-   0        0        0     4794 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/test/test_context.py
+-rw-rw-rw-   0        0        0     2445 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/test/test_file.py
+-rw-rw-rw-   0        0        0     1680 2024-02-20 09:04:57.000000 groupdocs-conversion-cloud-24.4/test/test_settings.py
```

### Comparing `groupdocs-conversion-cloud-24.2/LICENSE` & `groupdocs-conversion-cloud-24.4/LICENSE`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/PKG-INFO` & `groupdocs-conversion-cloud-24.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groupdocs-conversion-cloud
-Version: 24.2
+Version: 24.4
 Summary: GroupDocs.Conversion Cloud Python SDK
 Home-page: http://github.com/groupdocs-conversion-cloud/groupdocs-conversion-cloud-python
 Author: GroupDocs
 Author-email: support@groupdocs.cloud
 Keywords: groupdocs,conversion,cloud,python,sdk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `groupdocs-conversion-cloud-24.2/README.md` & `groupdocs-conversion-cloud-24.4/README.md`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/__init__.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 from groupdocs_conversion_cloud.models.web_convert_options import WebConvertOptions
 from groupdocs_conversion_cloud.models.web_load_options import WebLoadOptions
 from groupdocs_conversion_cloud.models.word_processing_convert_options import WordProcessingConvertOptions
 from groupdocs_conversion_cloud.models.word_processing_load_options import WordProcessingLoadOptions
 from groupdocs_conversion_cloud.models.xml_load_options import XmlLoadOptions
 from groupdocs_conversion_cloud.models.bmp_convert_options import BmpConvertOptions
 from groupdocs_conversion_cloud.models.bmp_load_options import BmpLoadOptions
+from groupdocs_conversion_cloud.models.cf2_load_options import Cf2LoadOptions
 from groupdocs_conversion_cloud.models.csv_load_options import CsvLoadOptions
 from groupdocs_conversion_cloud.models.dcm_convert_options import DcmConvertOptions
 from groupdocs_conversion_cloud.models.dcm_load_options import DcmLoadOptions
 from groupdocs_conversion_cloud.models.dgn_load_options import DgnLoadOptions
 from groupdocs_conversion_cloud.models.djvu_convert_options import DjvuConvertOptions
 from groupdocs_conversion_cloud.models.dng_convert_options import DngConvertOptions
 from groupdocs_conversion_cloud.models.dng_load_options import DngLoadOptions
@@ -88,15 +89,17 @@
 from groupdocs_conversion_cloud.models.dot_convert_options import DotConvertOptions
 from groupdocs_conversion_cloud.models.dot_load_options import DotLoadOptions
 from groupdocs_conversion_cloud.models.dotm_convert_options import DotmConvertOptions
 from groupdocs_conversion_cloud.models.dotm_load_options import DotmLoadOptions
 from groupdocs_conversion_cloud.models.dotx_convert_options import DotxConvertOptions
 from groupdocs_conversion_cloud.models.dotx_load_options import DotxLoadOptions
 from groupdocs_conversion_cloud.models.dwf_load_options import DwfLoadOptions
+from groupdocs_conversion_cloud.models.dwfx_load_options import DwfxLoadOptions
 from groupdocs_conversion_cloud.models.dwg_load_options import DwgLoadOptions
+from groupdocs_conversion_cloud.models.dwt_load_options import DwtLoadOptions
 from groupdocs_conversion_cloud.models.dxf_load_options import DxfLoadOptions
 from groupdocs_conversion_cloud.models.emf_convert_options import EmfConvertOptions
 from groupdocs_conversion_cloud.models.emf_load_options import EmfLoadOptions
 from groupdocs_conversion_cloud.models.eml_load_options import EmlLoadOptions
 from groupdocs_conversion_cloud.models.emlx_load_options import EmlxLoadOptions
 from groupdocs_conversion_cloud.models.gif_convert_options import GifConvertOptions
 from groupdocs_conversion_cloud.models.gif_load_options import GifLoadOptions
```

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/api_client.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,20 +70,20 @@
     }
 
     def __init__(self, configuration, header_name=None, header_value=None,
                  cookie=None):
         self.configuration = configuration
         self.pool = None
         self.rest_client = rest.RESTClientObject(configuration)
-        self.default_headers = {'x-groupdocs-client': 'python sdk', 'x-groupdocs-version': '24.2'}
+        self.default_headers = {'x-groupdocs-client': 'python sdk', 'x-groupdocs-version': '24.4'}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'python sdk 24.2'
+        self.user_agent = 'python sdk 24.4'
 
     def __del__(self):
         if self.pool is not None:
             self.pool.close()
             self.pool.join()
 
     @property
```

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/api_exception.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/api_exception.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/apis/convert_api.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/apis/convert_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/apis/file_api.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/apis/file_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/apis/folder_api.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/apis/folder_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/apis/info_api.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/apis/info_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/apis/license_api.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/apis/license_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/apis/storage_api.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/apis/storage_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/auth.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/auth.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/configuration.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,10 +198,10 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 24.2\n"\
-               "SDK Package Version: 24.2".\
+               "Version of the API: 24.4\n"\
+               "SDK Package Version: 24.4".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/__init__.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 from groupdocs_conversion_cloud.models.web_convert_options import WebConvertOptions
 from groupdocs_conversion_cloud.models.web_load_options import WebLoadOptions
 from groupdocs_conversion_cloud.models.word_processing_convert_options import WordProcessingConvertOptions
 from groupdocs_conversion_cloud.models.word_processing_load_options import WordProcessingLoadOptions
 from groupdocs_conversion_cloud.models.xml_load_options import XmlLoadOptions
 from groupdocs_conversion_cloud.models.bmp_convert_options import BmpConvertOptions
 from groupdocs_conversion_cloud.models.bmp_load_options import BmpLoadOptions
+from groupdocs_conversion_cloud.models.cf2_load_options import Cf2LoadOptions
 from groupdocs_conversion_cloud.models.csv_load_options import CsvLoadOptions
 from groupdocs_conversion_cloud.models.dcm_convert_options import DcmConvertOptions
 from groupdocs_conversion_cloud.models.dcm_load_options import DcmLoadOptions
 from groupdocs_conversion_cloud.models.dgn_load_options import DgnLoadOptions
 from groupdocs_conversion_cloud.models.djvu_convert_options import DjvuConvertOptions
 from groupdocs_conversion_cloud.models.dng_convert_options import DngConvertOptions
 from groupdocs_conversion_cloud.models.dng_load_options import DngLoadOptions
@@ -66,15 +67,17 @@
 from groupdocs_conversion_cloud.models.dot_convert_options import DotConvertOptions
 from groupdocs_conversion_cloud.models.dot_load_options import DotLoadOptions
 from groupdocs_conversion_cloud.models.dotm_convert_options import DotmConvertOptions
 from groupdocs_conversion_cloud.models.dotm_load_options import DotmLoadOptions
 from groupdocs_conversion_cloud.models.dotx_convert_options import DotxConvertOptions
 from groupdocs_conversion_cloud.models.dotx_load_options import DotxLoadOptions
 from groupdocs_conversion_cloud.models.dwf_load_options import DwfLoadOptions
+from groupdocs_conversion_cloud.models.dwfx_load_options import DwfxLoadOptions
 from groupdocs_conversion_cloud.models.dwg_load_options import DwgLoadOptions
+from groupdocs_conversion_cloud.models.dwt_load_options import DwtLoadOptions
 from groupdocs_conversion_cloud.models.dxf_load_options import DxfLoadOptions
 from groupdocs_conversion_cloud.models.emf_convert_options import EmfConvertOptions
 from groupdocs_conversion_cloud.models.emf_load_options import EmfLoadOptions
 from groupdocs_conversion_cloud.models.eml_load_options import EmlLoadOptions
 from groupdocs_conversion_cloud.models.emlx_load_options import EmlxLoadOptions
 from groupdocs_conversion_cloud.models.gif_convert_options import GifConvertOptions
 from groupdocs_conversion_cloud.models.gif_load_options import GifLoadOptions
```

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/api_error.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/api_error.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/api_error_response.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/api_error_response.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/bmp_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/bmp_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/bmp_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/bmp_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/cad_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/cad_load_options.py`

 * *Files 18% similar despite different names*

```diff
@@ -41,120 +41,126 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'width': 'int',
-        'height': 'int',
-        'layout_names': 'list[str]'
+        'layout_names': 'list[str]',
+        'background_color': 'str',
+        'draw_type': 'str'
     }
 
     attribute_map = {
-        'width': 'Width',
-        'height': 'Height',
-        'layout_names': 'LayoutNames'
+        'layout_names': 'LayoutNames',
+        'background_color': 'BackgroundColor',
+        'draw_type': 'DrawType'
     }
 
-    def __init__(self, width=None, height=None, layout_names=None, **kwargs):  # noqa: E501
+    def __init__(self, layout_names=None, background_color=None, draw_type=None, **kwargs):  # noqa: E501
         """Initializes new instance of CadLoadOptions"""  # noqa: E501
 
-        self._width = None
-        self._height = None
         self._layout_names = None
+        self._background_color = None
+        self._draw_type = None
 
-        if width is not None:
-            self.width = width
-        if height is not None:
-            self.height = height
         if layout_names is not None:
             self.layout_names = layout_names
+        if background_color is not None:
+            self.background_color = background_color
+        if draw_type is not None:
+            self.draw_type = draw_type
 
         base = super(CadLoadOptions, self)
         base.__init__(**kwargs)
 
         self.swagger_types.update(base.swagger_types)
         self.attribute_map.update(base.attribute_map)
     
     @property
-    def width(self):
+    def layout_names(self):
         """
-        Gets the width.  # noqa: E501
+        Gets the layout_names.  # noqa: E501
 
-        Set desired page width for converting CAD document  # noqa: E501
+        Render specific CAD layouts  # noqa: E501
 
-        :return: The width.  # noqa: E501
-        :rtype: int
+        :return: The layout_names.  # noqa: E501
+        :rtype: list[str]
         """
-        return self._width
+        return self._layout_names
 
-    @width.setter
-    def width(self, width):
+    @layout_names.setter
+    def layout_names(self, layout_names):
         """
-        Sets the width.
+        Sets the layout_names.
 
-        Set desired page width for converting CAD document  # noqa: E501
+        Render specific CAD layouts  # noqa: E501
 
-        :param width: The width.  # noqa: E501
-        :type: int
+        :param layout_names: The layout_names.  # noqa: E501
+        :type: list[str]
         """
-        if width is None:
-            raise ValueError("Invalid value for `width`, must not be `None`")  # noqa: E501
-        self._width = width
+        self._layout_names = layout_names
     
     @property
-    def height(self):
+    def background_color(self):
         """
-        Gets the height.  # noqa: E501
+        Gets the background_color.  # noqa: E501
 
-        Set desired page height for converting CAD document  # noqa: E501
+        Gets or sets a background color.  # noqa: E501
 
-        :return: The height.  # noqa: E501
-        :rtype: int
+        :return: The background_color.  # noqa: E501
+        :rtype: str
         """
-        return self._height
+        return self._background_color
 
-    @height.setter
-    def height(self, height):
+    @background_color.setter
+    def background_color(self, background_color):
         """
-        Sets the height.
+        Sets the background_color.
 
-        Set desired page height for converting CAD document  # noqa: E501
+        Gets or sets a background color.  # noqa: E501
 
-        :param height: The height.  # noqa: E501
-        :type: int
+        :param background_color: The background_color.  # noqa: E501
+        :type: str
         """
-        if height is None:
-            raise ValueError("Invalid value for `height`, must not be `None`")  # noqa: E501
-        self._height = height
+        self._background_color = background_color
     
     @property
-    def layout_names(self):
+    def draw_type(self):
         """
-        Gets the layout_names.  # noqa: E501
+        Gets the draw_type.  # noqa: E501
 
-        Render specific CAD layouts  # noqa: E501
+        Gets or sets type of drawing.  # noqa: E501
 
-        :return: The layout_names.  # noqa: E501
-        :rtype: list[str]
+        :return: The draw_type.  # noqa: E501
+        :rtype: str
         """
-        return self._layout_names
+        return self._draw_type
 
-    @layout_names.setter
-    def layout_names(self, layout_names):
+    @draw_type.setter
+    def draw_type(self, draw_type):
         """
-        Sets the layout_names.
+        Sets the draw_type.
 
-        Render specific CAD layouts  # noqa: E501
+        Gets or sets type of drawing.  # noqa: E501
 
-        :param layout_names: The layout_names.  # noqa: E501
-        :type: list[str]
+        :param draw_type: The draw_type.  # noqa: E501
+        :type: str
         """
-        self._layout_names = layout_names
+        if draw_type is None:
+            raise ValueError("Invalid value for `draw_type`, must not be `None`")  # noqa: E501
+        allowed_values = ["UseDrawColor", "UseObjectColor"]  # noqa: E501
+        if not draw_type.isdigit():	
+            if draw_type not in allowed_values:
+                raise ValueError(
+                    "Invalid value for `draw_type` ({0}), must be one of {1}"  # noqa: E501
+                    .format(draw_type, allowed_values))
+            self._draw_type = draw_type
+        else:
+            self._draw_type = allowed_values[int(draw_type) if six.PY3 else long(draw_type)]
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
```

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/consumption_result.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/consumption_result.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/convert_settings.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/convert_settings.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/csv_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/csv_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/dcm_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dcm_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/dcm_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dcm_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/dgn_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dgn_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/diagram_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/diagram_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/disc_usage.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/disc_usage.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/djvu_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/djvu_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/dng_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dng_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/dng_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dng_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/doc_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/doc_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/doc_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/doc_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/docm_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/docm_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/docm_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/docm_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/document_metadata.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/document_metadata.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/docx_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/docx_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/docx_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/docx_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/dot_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dot_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/dot_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dot_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/dotm_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dotm_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/dotm_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dotm_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/dotx_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dotx_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/dotx_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dotx_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/dwf_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dwf_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/dwg_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dwg_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/dxf_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/dxf_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/e_book_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/e_book_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/email_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/email_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/emf_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/emf_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/emf_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/emf_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/eml_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/eml_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/emlx_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/emlx_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/error.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/error.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/error_details.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/error_details.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/field_label.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/field_label.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/file_version.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/file_version.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/file_versions.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/file_versions.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/files_list.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/files_list.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/files_upload_result.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/files_upload_result.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/gif_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/gif_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/gif_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/gif_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ico_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ico_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ico_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ico_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ifc_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ifc_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/igs_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/igs_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/image_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/image_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/image_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/image_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/j2c_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/j2c_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/j2c_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/j2c_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/j2k_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/j2k_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/j2k_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/j2k_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/jp2_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/jp2_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/jp2_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/jp2_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/jpeg_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/jpeg_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/jpeg_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/jpeg_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/jpf_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/jpf_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/jpf_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/jpf_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/jpg_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/jpg_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/jpg_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/jpg_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/jpm_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/jpm_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/jpm_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/jpm_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/jpx_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/jpx_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/jpx_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/jpx_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/license_info.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/license_info.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/mht_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/mht_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/mobi_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/mobi_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/msg_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/msg_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/object_exist.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/object_exist.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/odg_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/odg_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/odg_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/odg_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/odp_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/odp_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/odp_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/odp_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ods_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ods_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ods_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ods_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/odt_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/odt_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/odt_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/odt_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/one_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/one_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ost_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ost_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/otp_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/otp_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/otp_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/otp_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ots_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ots_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ots_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ots_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ott_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ott_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ott_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ott_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/pdf_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/pdf_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/pdf_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/pdf_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/pdl_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/pdl_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/personal_storage_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/personal_storage_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/plt_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/plt_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/png_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/png_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/png_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/png_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/potm_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/potm_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/potm_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/potm_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/potx_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/potx_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/potx_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/potx_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/pps_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/pps_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/pps_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/pps_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ppsm_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ppsm_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ppsm_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ppsm_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ppsx_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ppsx_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ppsx_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ppsx_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ppt_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ppt_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/ppt_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/ppt_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/pptm_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/pptm_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/pptm_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/pptm_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/pptx_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/pptx_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/pptx_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/pptx_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/presentation_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/presentation_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/presentation_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/presentation_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/psd_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/psd_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/psd_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/psd_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/pst_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/pst_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/rtf_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/rtf_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/spreadsheet_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/spreadsheet_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/spreadsheet_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/spreadsheet_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/stl_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/stl_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/storage_exist.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/storage_exist.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/storage_file.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/storage_file.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/stored_converted_result.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/stored_converted_result.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/supported_format.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/supported_format.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/tif_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/tif_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/tif_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/tif_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/tiff_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/tiff_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/tiff_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/tiff_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/tsv_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/tsv_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/tsv_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/tsv_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/txt_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/txt_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/txt_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/txt_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/vdw_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/vdw_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/vdx_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/vdx_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/vsd_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/vsd_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/vsdm_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/vsdm_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/vsdx_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/vsdx_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/vss_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/vss_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/vssm_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/vssm_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/vssx_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/vssx_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/vst_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/vst_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/vstm_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/vstm_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/vstx_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/vstx_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/vsx_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/vsx_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/vtx_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/vtx_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/watermark_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/watermark_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/web_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/web_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/web_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/web_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/webp_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/webp_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/webp_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/webp_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/wmf_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/wmf_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/wmf_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/wmf_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/word_processing_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/word_processing_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/word_processing_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/word_processing_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xls2003_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xls2003_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xls2003_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xls2003_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xls_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xls_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xls_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xls_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xlsb_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xlsb_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xlsb_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xlsb_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xlsm_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xlsm_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xlsm_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xlsm_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xlsx_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xlsx_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xlsx_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xlsx_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xltm_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xltm_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xltm_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xltm_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xltx_convert_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xltx_convert_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xltx_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xltx_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/models/xml_load_options.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/models/xml_load_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud/rest.py` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud/rest.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud.egg-info/PKG-INFO` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groupdocs-conversion-cloud
-Version: 24.2
+Version: 24.4
 Summary: GroupDocs.Conversion Cloud Python SDK
 Home-page: http://github.com/groupdocs-conversion-cloud/groupdocs-conversion-cloud-python
 Author: GroupDocs
 Author-email: support@groupdocs.cloud
 Keywords: groupdocs,conversion,cloud,python,sdk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `groupdocs-conversion-cloud-24.2/groupdocs_conversion_cloud.egg-info/SOURCES.txt` & `groupdocs-conversion-cloud-24.4/groupdocs_conversion_cloud.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 groupdocs_conversion_cloud/apis/storage_api.py
 groupdocs_conversion_cloud/models/__init__.py
 groupdocs_conversion_cloud/models/api_error.py
 groupdocs_conversion_cloud/models/api_error_response.py
 groupdocs_conversion_cloud/models/bmp_convert_options.py
 groupdocs_conversion_cloud/models/bmp_load_options.py
 groupdocs_conversion_cloud/models/cad_load_options.py
+groupdocs_conversion_cloud/models/cf2_load_options.py
 groupdocs_conversion_cloud/models/consumption_result.py
 groupdocs_conversion_cloud/models/convert_options.py
 groupdocs_conversion_cloud/models/convert_settings.py
 groupdocs_conversion_cloud/models/csv_load_options.py
 groupdocs_conversion_cloud/models/dcm_convert_options.py
 groupdocs_conversion_cloud/models/dcm_load_options.py
 groupdocs_conversion_cloud/models/dgn_load_options.py
@@ -47,15 +48,17 @@
 groupdocs_conversion_cloud/models/dot_convert_options.py
 groupdocs_conversion_cloud/models/dot_load_options.py
 groupdocs_conversion_cloud/models/dotm_convert_options.py
 groupdocs_conversion_cloud/models/dotm_load_options.py
 groupdocs_conversion_cloud/models/dotx_convert_options.py
 groupdocs_conversion_cloud/models/dotx_load_options.py
 groupdocs_conversion_cloud/models/dwf_load_options.py
+groupdocs_conversion_cloud/models/dwfx_load_options.py
 groupdocs_conversion_cloud/models/dwg_load_options.py
+groupdocs_conversion_cloud/models/dwt_load_options.py
 groupdocs_conversion_cloud/models/dxf_load_options.py
 groupdocs_conversion_cloud/models/e_book_convert_options.py
 groupdocs_conversion_cloud/models/email_load_options.py
 groupdocs_conversion_cloud/models/emf_convert_options.py
 groupdocs_conversion_cloud/models/emf_load_options.py
 groupdocs_conversion_cloud/models/eml_load_options.py
 groupdocs_conversion_cloud/models/emlx_load_options.py
```

### Comparing `groupdocs-conversion-cloud-24.2/setup.py` & `groupdocs-conversion-cloud-24.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import sys
 import datetime
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "groupdocs-conversion-cloud"
-VERSION = "24.2"
+VERSION = "24.4"
 
 # Append current time to the version when publishing to test environment
 if "--test" in sys.argv:
     VERSION += "." + datetime.datetime.now().strftime("%Y%m%d%H%M")
     sys.argv.remove("--test")
 
 # To install the library, run the following
```

### Comparing `groupdocs-conversion-cloud-24.2/test/apis/test_auth_api.py` & `groupdocs-conversion-cloud-24.4/test/apis/test_auth_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/test/apis/test_convert_api.py` & `groupdocs-conversion-cloud-24.4/test/apis/test_convert_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/test/apis/test_file_api.py` & `groupdocs-conversion-cloud-24.4/test/apis/test_file_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/test/apis/test_folder_api.py` & `groupdocs-conversion-cloud-24.4/test/apis/test_folder_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/test/apis/test_info_api.py` & `groupdocs-conversion-cloud-24.4/test/apis/test_info_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/test/apis/test_storage_api.py` & `groupdocs-conversion-cloud-24.4/test/apis/test_storage_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/test/test_context.py` & `groupdocs-conversion-cloud-24.4/test/test_context.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/test/test_file.py` & `groupdocs-conversion-cloud-24.4/test/test_file.py`

 * *Files identical despite different names*

### Comparing `groupdocs-conversion-cloud-24.2/test/test_settings.py` & `groupdocs-conversion-cloud-24.4/test/test_settings.py`

 * *Files identical despite different names*

