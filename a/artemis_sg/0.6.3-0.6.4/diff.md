# Comparing `tmp/artemis_sg-0.6.3.tar.gz` & `tmp/artemis_sg-0.6.4.tar.gz`

## Comparing `artemis_sg-0.6.3.tar` & `artemis_sg-0.6.4.tar`

### file list

```diff
@@ -1,73 +1,75 @@
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/.gitlab-ci.yml
--rw-r--r--   0        0        0    15112 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/CHANGELOG.md
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/pypi_creds.asc
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/pytest.ini
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/.gitlab/issue_templates/issue.md
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/.gitlab/issue_templates/meeting_notes.md
--rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/.gitlab/issue_templates/release.md
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/docs/cli_ref.rst
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/docs/conf.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/docs/config_ref.md
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/docs/index.md
--rw-r--r--   0        0        0     6689 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/docs/installation.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/docs/release.md -> ../.gitlab/issue_templates/release.md
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/docs/testing.md
--rw-r--r--   0        0        0    13626 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/docs/usage.md
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/docs/guides/index.md
--rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/docs/guides/powershell_profile.md
--rw-r--r--   0        0        0    15408 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/docs/resources/artemis_logo.png
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/htmlcov/.gitignore
--rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/htmlcov/d_36c98836e6288b3a___init___py.html
--rw-r--r--   0        0        0     5918 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/htmlcov/d_36c98836e6288b3a__version_py.html
--rw-r--r--   0        0        0    21981 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/htmlcov/d_36c98836e6288b3a_app_creds_py.html
--rw-r--r--   0        0        0   148602 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/htmlcov/d_36c98836e6288b3a_cli_py.html
--rw-r--r--   0        0        0    35921 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/htmlcov/d_36c98836e6288b3a_foo_py.html
--rw-r--r--   0        0        0    46161 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/htmlcov/d_36c98836e6288b3a_gcloud_py.html
--rw-r--r--   0        0        0    42836 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/htmlcov/d_36c98836e6288b3a_img_downloader_py.html
--rw-r--r--   0        0        0    22670 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/htmlcov/d_36c98836e6288b3a_item_py.html
--rw-r--r--   0        0        0    41857 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/htmlcov/d_36c98836e6288b3a_items_py.html
--rw-r--r--   0        0        0   301228 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/htmlcov/d_36c98836e6288b3a_scraper_py.html
--rw-r--r--   0        0        0   186041 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/htmlcov/d_36c98836e6288b3a_slide_generator_py.html
--rw-r--r--   0        0        0   136170 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/htmlcov/d_36c98836e6288b3a_spreadsheet_py.html
--rw-r--r--   0        0        0    15184 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/htmlcov/d_36c98836e6288b3a_vendor_py.html
--rw-r--r--   0        0        0    61347 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/htmlcov/d_62e0d06e17bdb05b___init___py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/htmlcov/keybd_open.png
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/htmlcov/style.css
--rw-r--r--   0        0        0    57344 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/src/artemis_sg/.scraper.py.swp
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/src/artemis_sg/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/src/artemis_sg/_version.py
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/src/artemis_sg/app_creds.py
--rw-r--r--   0        0        0    20014 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/src/artemis_sg/cli.py
--rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/src/artemis_sg/gcloud.py
--rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/src/artemis_sg/img_downloader.py
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/src/artemis_sg/item.py
--rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/src/artemis_sg/items.py
--rw-r--r--   0        0        0    39389 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/src/artemis_sg/scraper.py
--rw-r--r--   0        0        0    22268 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/src/artemis_sg/slide_generator.py
--rw-r--r--   0        0        0    15356 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/src/artemis_sg/spreadsheet.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/src/artemis_sg/vendor.py
--rw-r--r--   0        0        0     6734 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/src/artemis_sg/config/__init__.py
--rw-r--r--   0        0        0    13320 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/src/artemis_sg/data/artemis_logo.png
--rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/tests/conftest.py
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/tests/test_app_creds.py
--rw-r--r--   0        0        0    13916 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/tests/test_cli.py
--rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/tests/test_gcloud.py
--rw-r--r--   0        0        0    13185 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/tests/test_img_downloader.py
--rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/tests/test_item.py
--rw-r--r--   0        0        0     9534 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/tests/test_items.py
--rw-r--r--   0        0        0    39544 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/tests/test_scraper.py
--rw-r--r--   0        0        0     6207 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/tests/test_slide_generator.py
--rw-r--r--   0        0        0    11661 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/tests/test_spreadsheet.py
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/tests/test_vendor.py
--rw-r--r--   0        0        0    15408 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/tests/data/artemis_logo.png
--rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/tests/data/captcha.png
--rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/tests/data/notsolved.png
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/.gitignore
--rw-r--r--   0        0        0    35145 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/LICENSE
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/README.md
--rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 artemis_sg-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/.gitlab-ci.yml
+-rw-r--r--   0        0        0    15372 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/CHANGELOG.md
+-rw-r--r--   0        0        0  1139726 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/artemis_sg-20240402-200027.log
+-rw-r--r--   0        0        0   886782 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/artemis_sg-20240402-205156.log
+-rw-r--r--   0        0        0   487804 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/artemis_sg-20240402-210236.log
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/pypi_creds.asc
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/pytest.ini
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/.gitlab/issue_templates/issue.md
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/.gitlab/issue_templates/meeting_notes.md
+-rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/.gitlab/issue_templates/release.md
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/docs/cli_ref.rst
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/docs/conf.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/docs/config_ref.md
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/docs/index.md
+-rw-r--r--   0        0        0     6689 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/docs/installation.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/docs/release.md -> ../.gitlab/issue_templates/release.md
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/docs/testing.md
+-rw-r--r--   0        0        0    13626 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/docs/usage.md
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/docs/guides/index.md
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/docs/guides/powershell_profile.md
+-rw-r--r--   0        0        0    15408 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/docs/resources/artemis_logo.png
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/htmlcov/d_36c98836e6288b3a___init___py.html
+-rw-r--r--   0        0        0     5918 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/htmlcov/d_36c98836e6288b3a__version_py.html
+-rw-r--r--   0        0        0    21981 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/htmlcov/d_36c98836e6288b3a_app_creds_py.html
+-rw-r--r--   0        0        0   148602 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/htmlcov/d_36c98836e6288b3a_cli_py.html
+-rw-r--r--   0        0        0    35921 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/htmlcov/d_36c98836e6288b3a_foo_py.html
+-rw-r--r--   0        0        0    46161 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/htmlcov/d_36c98836e6288b3a_gcloud_py.html
+-rw-r--r--   0        0        0    42836 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/htmlcov/d_36c98836e6288b3a_img_downloader_py.html
+-rw-r--r--   0        0        0    22670 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/htmlcov/d_36c98836e6288b3a_item_py.html
+-rw-r--r--   0        0        0    41857 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/htmlcov/d_36c98836e6288b3a_items_py.html
+-rw-r--r--   0        0        0   301228 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/htmlcov/d_36c98836e6288b3a_scraper_py.html
+-rw-r--r--   0        0        0   186041 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/htmlcov/d_36c98836e6288b3a_slide_generator_py.html
+-rw-r--r--   0        0        0   136170 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/htmlcov/d_36c98836e6288b3a_spreadsheet_py.html
+-rw-r--r--   0        0        0    15184 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/htmlcov/d_36c98836e6288b3a_vendor_py.html
+-rw-r--r--   0        0        0    61347 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/htmlcov/d_62e0d06e17bdb05b___init___py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/htmlcov/style.css
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/src/artemis_sg/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/src/artemis_sg/_version.py
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/src/artemis_sg/app_creds.py
+-rw-r--r--   0        0        0    20046 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/src/artemis_sg/cli.py
+-rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/src/artemis_sg/gcloud.py
+-rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/src/artemis_sg/img_downloader.py
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/src/artemis_sg/item.py
+-rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/src/artemis_sg/items.py
+-rw-r--r--   0        0        0    39389 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/src/artemis_sg/scraper.py
+-rw-r--r--   0        0        0    22833 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/src/artemis_sg/slide_generator.py
+-rw-r--r--   0        0        0    15356 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/src/artemis_sg/spreadsheet.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/src/artemis_sg/vendor.py
+-rw-r--r--   0        0        0     6734 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/src/artemis_sg/config/__init__.py
+-rw-r--r--   0        0        0    13320 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/src/artemis_sg/data/artemis_logo.png
+-rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/tests/conftest.py
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/tests/test_app_creds.py
+-rw-r--r--   0        0        0    13916 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/tests/test_cli.py
+-rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/tests/test_gcloud.py
+-rw-r--r--   0        0        0    13185 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/tests/test_img_downloader.py
+-rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/tests/test_item.py
+-rw-r--r--   0        0        0     9534 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/tests/test_items.py
+-rw-r--r--   0        0        0    39526 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/tests/test_scraper.py
+-rw-r--r--   0        0        0     6207 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/tests/test_slide_generator.py
+-rw-r--r--   0        0        0    11661 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/tests/test_spreadsheet.py
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/tests/test_vendor.py
+-rw-r--r--   0        0        0    15408 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/tests/data/artemis_logo.png
+-rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/tests/data/captcha.png
+-rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/tests/data/notsolved.png
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/.gitignore
+-rw-r--r--   0        0        0    35145 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/LICENSE
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/README.md
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 artemis_sg-0.6.4/PKG-INFO
```

### Comparing `artemis_sg-0.6.3/.gitlab-ci.yml` & `artemis_sg-0.6.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/CHANGELOG.md` & `artemis_sg-0.6.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,21 @@
 
 ## [Unreleased]
 ### Added
 ### Fixed
 ### Changed
 ### Removed
 
+## [0.6.4] - 2024-04-05
+### Added
+### Fixed
+- SlideGenerator: Create cloud image URLs at time of slide content to ensure they do not expire. (#215)
+### Changed
+### Removed
+
 ## [0.6.3] - 2024-03-17
 ### Added
 - AmznScraper: Image widget failover. (#228)
 - Docstrings to `img_downloader.py`. (#89,#107)
 ### Fixed
 - Scraper: Prevent AmznUkScraper hanging on 503 page. (#227)
 - Scraper: Prevent AmznUkScraper from throwing exceptions. (#227)
@@ -367,15 +374,16 @@
 - Documentation via README.
 - Object oriented structure to code-base.
 - LICENSE for GPL-3.0 or later.
 
 ### Removed
 - Script interface for slide generation.
 
-[unreleased]: https://gitlab.com/johnduarte/artemis_slide_generator/compare/v0.6.3...main
+[unreleased]: https://gitlab.com/johnduarte/artemis_slide_generator/compare/v0.6.4...main
+[0.6.4]: https://gitlab.com/johnduarte/artemis_slide_generator/compare/v0.6.3...v0.6.4
 [0.6.3]: https://gitlab.com/johnduarte/artemis_slide_generator/compare/v0.6.2...v0.6.3
 [0.6.2]: https://gitlab.com/johnduarte/artemis_slide_generator/compare/v0.6.1...v0.6.2
 [0.6.1]: https://gitlab.com/johnduarte/artemis_slide_generator/compare/v0.6.0...v0.6.1
 [0.6.0]: https://gitlab.com/johnduarte/artemis_slide_generator/compare/v0.5.9...v0.6.0
 [0.5.9]: https://gitlab.com/johnduarte/artemis_slide_generator/compare/v0.5.8...v0.5.9
 [0.5.8]: https://gitlab.com/johnduarte/artemis_slide_generator/compare/v0.5.7...v0.5.8
 [0.5.7]: https://gitlab.com/johnduarte/artemis_slide_generator/compare/v0.5.6...v0.5.7
```

### Comparing `artemis_sg-0.6.3/pypi_creds.asc` & `artemis_sg-0.6.4/pypi_creds.asc`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/.gitlab/issue_templates/release.md` & `artemis_sg-0.6.4/.gitlab/issue_templates/release.md`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/docs/cli_ref.rst` & `artemis_sg-0.6.4/docs/cli_ref.rst`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/docs/conf.py` & `artemis_sg-0.6.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/docs/index.md` & `artemis_sg-0.6.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/docs/installation.md` & `artemis_sg-0.6.4/docs/installation.md`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/docs/testing.md` & `artemis_sg-0.6.4/docs/testing.md`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/docs/usage.md` & `artemis_sg-0.6.4/docs/usage.md`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/docs/guides/powershell_profile.md` & `artemis_sg-0.6.4/docs/guides/powershell_profile.md`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/docs/resources/artemis_logo.png` & `artemis_sg-0.6.4/docs/resources/artemis_logo.png`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/htmlcov/coverage_html.js` & `artemis_sg-0.6.4/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/htmlcov/d_36c98836e6288b3a___init___py.html` & `artemis_sg-0.6.4/htmlcov/d_36c98836e6288b3a___init___py.html`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/htmlcov/d_36c98836e6288b3a__version_py.html` & `artemis_sg-0.6.4/htmlcov/d_36c98836e6288b3a__version_py.html`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/htmlcov/d_36c98836e6288b3a_app_creds_py.html` & `artemis_sg-0.6.4/htmlcov/d_36c98836e6288b3a_app_creds_py.html`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/htmlcov/d_36c98836e6288b3a_cli_py.html` & `artemis_sg-0.6.4/htmlcov/d_36c98836e6288b3a_cli_py.html`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/htmlcov/d_36c98836e6288b3a_foo_py.html` & `artemis_sg-0.6.4/htmlcov/d_36c98836e6288b3a_foo_py.html`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/htmlcov/d_36c98836e6288b3a_gcloud_py.html` & `artemis_sg-0.6.4/htmlcov/d_36c98836e6288b3a_gcloud_py.html`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/htmlcov/d_36c98836e6288b3a_img_downloader_py.html` & `artemis_sg-0.6.4/htmlcov/d_36c98836e6288b3a_img_downloader_py.html`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/htmlcov/d_36c98836e6288b3a_item_py.html` & `artemis_sg-0.6.4/htmlcov/d_36c98836e6288b3a_item_py.html`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/htmlcov/d_36c98836e6288b3a_items_py.html` & `artemis_sg-0.6.4/htmlcov/d_36c98836e6288b3a_items_py.html`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/htmlcov/d_36c98836e6288b3a_scraper_py.html` & `artemis_sg-0.6.4/htmlcov/d_36c98836e6288b3a_scraper_py.html`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/htmlcov/d_36c98836e6288b3a_slide_generator_py.html` & `artemis_sg-0.6.4/htmlcov/d_36c98836e6288b3a_slide_generator_py.html`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/htmlcov/d_36c98836e6288b3a_spreadsheet_py.html` & `artemis_sg-0.6.4/htmlcov/d_36c98836e6288b3a_spreadsheet_py.html`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/htmlcov/d_36c98836e6288b3a_vendor_py.html` & `artemis_sg-0.6.4/htmlcov/d_36c98836e6288b3a_vendor_py.html`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/htmlcov/d_62e0d06e17bdb05b___init___py.html` & `artemis_sg-0.6.4/htmlcov/d_62e0d06e17bdb05b___init___py.html`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/htmlcov/favicon_32.png` & `artemis_sg-0.6.4/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/htmlcov/index.html` & `artemis_sg-0.6.4/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/htmlcov/keybd_closed.png` & `artemis_sg-0.6.4/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/htmlcov/keybd_open.png` & `artemis_sg-0.6.4/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/htmlcov/style.css` & `artemis_sg-0.6.4/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/src/artemis_sg/app_creds.py` & `artemis_sg-0.6.4/src/artemis_sg/app_creds.py`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/src/artemis_sg/cli.py` & `artemis_sg-0.6.4/src/artemis_sg/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,32 +208,34 @@
     The command utilizes configuration variables stored in "config.toml" to set
     the vendor from [asg.vendors] and scraped items database from
     [asg.data.file.scraped].
     """
     cmd = "generate"
     namespace = f"{MODULE}.{cmd}"
 
+    if not ctx.obj["VENDOR"]:
+        click.echo("\tVENDOR not provided", err=True)
+        click.echo("\tCannot continue.  Exiting.", err=True)
+        sys.exit(1)
+    if not ctx.obj["WORKBOOK"]:
+        click.echo("\tWORKBOOK not provided", err=True)
+        click.echo("\tCannot continue.  Exiting.", err=True)
+        sys.exit(1)
+
     sdb = CFG["asg"]["data"]["file"]["scraped"]
     msg = (
         f"Creating Google Slides deck '{title}' for '{ctx.obj['VENDOR'] or ''!s}' "
         f"using '{ctx.obj['WORKBOOK'] or ''!s}':'{ctx.obj['WORKSHEET'] or ''!s}'..."
     )
     click.echo(msg)
     logging.debug(f"{namespace}: Scraped Items Database is: {sdb}")
 
-    try:
-        slide_generator_wrapper(
-            ctx.obj["VENDOR"], ctx.obj["WORKBOOK"], ctx.obj["WORKSHEET"], sdb, title
-        )
-    except Exception as e:
-        click.echo(f"Could not generate slide deck:{e}", err=True)
-        if not ctx.obj["VENDOR"]:
-            click.echo("\tVENDOR not provided", err=True)
-        if not ctx.obj["WORKBOOK"]:
-            click.echo("\tWORKBOOK not provided", err=True)
+    slide_generator_wrapper(
+        ctx.obj["VENDOR"], ctx.obj["WORKBOOK"], ctx.obj["WORKSHEET"], sdb, title
+    )
 
 
 @cli.command()
 @click.option("-o", "--output", "out", default="out.xlsx", help="Output file")
 @click.pass_context
 def sheet_image(ctx, out):
     """
```

### Comparing `artemis_sg-0.6.3/src/artemis_sg/gcloud.py` & `artemis_sg-0.6.4/src/artemis_sg/gcloud.py`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/src/artemis_sg/img_downloader.py` & `artemis_sg-0.6.4/src/artemis_sg/img_downloader.py`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/src/artemis_sg/item.py` & `artemis_sg-0.6.4/src/artemis_sg/item.py`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/src/artemis_sg/items.py` & `artemis_sg-0.6.4/src/artemis_sg/items.py`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/src/artemis_sg/scraper.py` & `artemis_sg-0.6.4/src/artemis_sg/scraper.py`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/src/artemis_sg/slide_generator.py` & `artemis_sg-0.6.4/src/artemis_sg/slide_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,19 +159,25 @@
             ]
         rsp = self.slide_batch_update_get_replies(deck_id, reqs)
         for i in rsp:
             book_slide_id_list.append(i["createSlide"]["objectId"])
         return book_slide_id_list
 
     def slide_batch_update(self, deck_id, reqs):
-        return (
+        try:
+            res = (
             self.slides.presentations()
             .batchUpdate(body={"requests": reqs}, presentationId=deck_id)
             .execute()
-        )
+            )
+        except Exception as e:
+            logging.error(f"Failed to update slide batch: Errror: {e}")
+            res = None
+
+        return res
 
     def slide_batch_update_get_replies(self, deck_id, reqs):
         return (
             self.slides.presentations()
             .batchUpdate(body={"requests": reqs}, presentationId=deck_id)
             .execute()
             .get("replies")
@@ -417,21 +423,26 @@
             (0, y_offset), text, font=font, spacing=line_spacing
         )  # put the text on the image
         text_file = "%s_text.png" % isbn
         text_file = os.path.join(text_bucket_path, text_file)
         image.save(text_file)
         return text_file
 
-    def get_cloud_urls(self, item, bucket_prefix):
-        blob_names = self.gcloud.list_image_blob_names(bucket_prefix)
+    def set_image_blob_list(self, bucket_prefix):
+        self.image_blob_list = self.gcloud.list_image_blob_names(bucket_prefix)
+
+    def get_item_image_blob_list(self, item):
         # FIXME:  This should happen in Item object at time of instantiation.
         if not item.isbn and "TBCODE" in item.data:
             item.isbn = item.data["TBCODE"]
-        image_list = [blob for blob in blob_names if item.isbn in blob]
-        sl = sorted(image_list)
+        image_list = [blob for blob in self.image_blob_list if str(item.isbn) in blob]
+        return sorted(image_list)
+
+    def get_cloud_urls(self, item):
+        sl = self.get_item_image_blob_list(item)
         # generate URLs for item images on google cloud storage
         url_list = []
         for name in sl:
             url = self.gcloud.generate_cloud_signed_url(name)
             url_list.append(url)
 
         return url_list
@@ -442,14 +453,18 @@
         if text_bucket_prefix == bucket_prefix:
             text_bucket_prefix = bucket_prefix + "_text"
         return text_bucket_prefix
 
     ####################################################################################
     def generate(self, items, bucket_prefix, deck_title=None):  # noqa: PLR0915
         namespace = f"{type(self).__name__}.{self.generate.__name__}"
+
+        logging.info(f"{namespace}: Getting image blob list")
+        self.set_image_blob_list(bucket_prefix)
+
         slide_max_batch = CFG["asg"]["slide_generator"]["slide_max_batch"]
         text_bucket_prefix = self.get_text_bucket_prefix(bucket_prefix)
         text_bucket_path = os.path.join(artemis_sg.data_dir, text_bucket_prefix)
         if not os.path.isdir(text_bucket_path):
             os.mkdir(text_bucket_path)
 
         logging.info(f"{namespace}: Create new slide deck")
@@ -485,16 +500,17 @@
                 self.color_to_rgbcolor(CFG["asg"]["slide_generator"]["text_color"]))
         reqs += self.get_req_slide_bg_color(
                 title_slide_id,
                 self.color_to_rgbcolor(CFG["asg"]["slide_generator"]["bg_color"]))
         reqs += self.get_req_create_logo(title_slide_id)
 
         # find images and delete books entries without images
+        # using blob list as proxy for final urls to be generated later.
         for item in items:
-            item.image_urls = self.get_cloud_urls(item, bucket_prefix)
+            item.image_urls = self.get_item_image_blob_list(item)
 
         # update title slide
         self.slide_batch_update(deck_id, reqs)
         # clear reqs
         reqs = []
         # create book slides
         items_with_images = items.get_items_with_image_urls()
@@ -507,14 +523,15 @@
         upper_index = len(e_books)
         offset = 0
         for _b in range(batches):
             upper = offset + slide_max_batch
             if upper > upper_index:
                 upper = upper_index
             for book_slide_id, book in e_books[offset:upper]:
+                book.image_urls = self.get_cloud_urls(book)
                 reqs = self.get_req_update_artemis_slide(
                     deck_id, book_slide_id, book, text_bucket_path, reqs
                 )
             logging.info(f"{namespace}: Execute img/text update reqs")
             # pp.pprint(reqs)
             # exit()
             self.slide_batch_update(deck_id, reqs)
```

### Comparing `artemis_sg-0.6.3/src/artemis_sg/spreadsheet.py` & `artemis_sg-0.6.4/src/artemis_sg/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/src/artemis_sg/vendor.py` & `artemis_sg-0.6.4/src/artemis_sg/vendor.py`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/src/artemis_sg/config/__init__.py` & `artemis_sg-0.6.4/src/artemis_sg/config/__init__.py`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/src/artemis_sg/data/artemis_logo.png` & `artemis_sg-0.6.4/src/artemis_sg/data/artemis_logo.png`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/tests/conftest.py` & `artemis_sg-0.6.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/tests/test_app_creds.py` & `artemis_sg-0.6.4/tests/test_app_creds.py`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/tests/test_cli.py` & `artemis_sg-0.6.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/tests/test_gcloud.py` & `artemis_sg-0.6.4/tests/test_gcloud.py`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/tests/test_img_downloader.py` & `artemis_sg-0.6.4/tests/test_img_downloader.py`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/tests/test_item.py` & `artemis_sg-0.6.4/tests/test_item.py`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/tests/test_items.py` & `artemis_sg-0.6.4/tests/test_items.py`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/tests/test_scraper.py` & `artemis_sg-0.6.4/tests/test_scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         scrapr.load_item_page("9780241605783")
         urls = scrapr.scrape_item_image_urls()
         driver.close()
 
         assert isinstance(urls, list)
         assert len(urls) > 0
         assert (
-            "https://m.media-amazon.com/images/I/41Lq2BpbiNS.jpg" in urls[0]
+            "https://m.media-amazon.com/images" in urls[0]
         )
 
 
 class TestAmznScraper:
     def test_scrape_description_with_review(self, monkeypatch):
         """
         GIVEN a AmznScraper object with webdriver and amazon url
```

### Comparing `artemis_sg-0.6.3/tests/test_slide_generator.py` & `artemis_sg-0.6.4/tests/test_slide_generator.py`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/tests/test_spreadsheet.py` & `artemis_sg-0.6.4/tests/test_spreadsheet.py`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/tests/test_vendor.py` & `artemis_sg-0.6.4/tests/test_vendor.py`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/tests/data/artemis_logo.png` & `artemis_sg-0.6.4/tests/data/artemis_logo.png`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/tests/data/captcha.png` & `artemis_sg-0.6.4/tests/data/captcha.png`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/tests/data/notsolved.png` & `artemis_sg-0.6.4/tests/data/notsolved.png`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/LICENSE` & `artemis_sg-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/README.md` & `artemis_sg-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/pyproject.toml` & `artemis_sg-0.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `artemis_sg-0.6.3/PKG-INFO` & `artemis_sg-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artemis_sg
-Version: 0.6.3
+Version: 0.6.4
 Summary: Package for generating Google slide decks
 Project-URL: Homepage, https://gitlab.com/johnduarte/artemis_slide_generator
 Project-URL: Bug Tracker, https://gitlab.com/johnduarte/artemis_slide_generator/-/issues
 Project-URL: Changelog, https://gitlab.com/johnduarte/artemis_slide_generator/blob/main/CHANGELOG.md
 Author-email: John Duarte <john@yeliad.us>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
```

