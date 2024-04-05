# Comparing `tmp/aa_fleetpings-3.0.0.tar.gz` & `tmp/aa_fleetpings-3.0.0b1.tar.gz`

## Comparing `aa_fleetpings-3.0.0.tar` & `aa_fleetpings-3.0.0b1.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/__init__.py
--rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/admin.py
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/app_settings.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/apps.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/auth_hooks.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/constants.py
--rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/form.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/managers.py
--rw-r--r--   0        0        0    17339 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/models.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/urls.py
--rw-r--r--   0        0        0    13953 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/views.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/helper/discord_webhook.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/helper/eve_images.py
--rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/helper/ping_context.py
--rw-r--r--   0        0        0    13803 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/locale/django.pot
--rw-r--r--   0        0        0    14182 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    19835 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    22749 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14180 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    13947 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    13940 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    11650 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    22125 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    17350 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    23453 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    10965 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    24381 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14245 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    12854 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/migrations/0001_initial.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/migrations/0002_webhook_is_embed_description_change.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/migrations/0003_fleetdoctrine_link.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/migrations/0004_auto_20200915_1617.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/migrations/0005_fleettype_restricted_to_group.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/migrations/0006_fleetdoctrine_restricted_to_group.py
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/migrations/0007_mysql8_default_value_fixes_20201003_1232.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/migrations/0008_auto_20210114_1733.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/migrations/0009_remove_webhook_is_embedded_remove_webhook_type_and_more.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/migrations/0010_use_ellipsis_character_in_strings.py
--rw-r--r--   0        0        0    12638 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/migrations/0011_settings_and_verbose_names.py
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/migrations/0012_migrate_app_settings_from_local_py_to_database.py
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/migrations/0013_fleetcomm_channel.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/migrations/0014_update_models.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/migrations/0015_alter_discordpingtarget_options_and_more.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/migrations/__init__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/static/fleetpings/css/fleetpings.css
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/static/fleetpings/css/fleetpings.min.css
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/static/fleetpings/css/fleetpings.min.css.map
--rw-r--r--   0        0        0    15722 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/static/fleetpings/js/fleetpings.js
--rw-r--r--   0        0        0     5551 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/static/fleetpings/js/fleetpings.min.js
--rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/static/fleetpings/js/fleetpings.min.js.map
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/static/fleetpings/libs/flexdatalist/2.3.0/LICENSE
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/static/fleetpings/libs/flexdatalist/2.3.0/README.md
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/static/fleetpings/libs/flexdatalist/2.3.0/jquery.flexdatalist.css
--rw-r--r--   0        0        0    77378 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/static/fleetpings/libs/flexdatalist/2.3.0/jquery.flexdatalist.js
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/static/fleetpings/libs/flexdatalist/2.3.0/jquery.flexdatalist.min.css
--rw-r--r--   0        0        0    24873 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/static/fleetpings/libs/flexdatalist/2.3.0/jquery.flexdatalist.min.js
--rw-r--r--   0        0        0    23171 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/static/fleetpings/libs/flexdatalist/2.3.0/jquery.flexdatalist.min.js.map
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/base.html
--rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/index.html
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/bundles/fleetpings-css.html
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/bundles/fleetpings-js.html
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/bundles/flexdatalist-css.html
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/bundles/flexdatalist-js.html
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/partials/form/form.html
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/partials/form/segments/fleet-comms.html
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/partials/form/segments/fleet-doctrine.html
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/partials/form/segments/fleet-formup-location.html
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/partials/form/segments/fleet-type-loop.html
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/partials/form/segments/fleet-type.html
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/partials/form/segments/ping-channel.html
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/partials/form/segments/ping-targets-loop.html
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/partials/form/segments/ping-targets.html
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/partials/header/page-header.html
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/partials/ping/copy-paste-text.html
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/partials/ping/ping.html
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/templatetags/__init__.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/templatetags/fleetpings.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/tests/__init__.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/tests/test_access.py
--rw-r--r--   0        0        0    12747 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/tests/test_ajax_calls.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/tests/test_auth_hooks.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/tests/test_helper_eve_images.py
--rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/tests/test_installed_modules.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/tests/test_model_discprdpingtarget.py
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/tests/test_model_fleetcomm.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/tests/test_model_fleetdoctrine.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/tests/test_model_fleettype.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/tests/test_model_formuplocation.py
--rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/tests/test_model_setting.py
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/tests/test_model_webhook.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/tests/test_templatetags.py
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/fleetpings/tests/utils.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/LICENSE
--rw-r--r--   0        0        0     8656 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/README.md
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/pyproject.toml
--rw-r--r--   0        0        0    51307 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/__init__.py
+-rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/admin.py
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/app_settings.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/apps.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/auth_hooks.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/constants.py
+-rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/form.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/managers.py
+-rw-r--r--   0        0        0    17339 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/models.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/urls.py
+-rw-r--r--   0        0        0    13953 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/views.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/helper/discord_webhook.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/helper/eve_images.py
+-rw-r--r--   0        0        0     8302 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/helper/ping_context.py
+-rw-r--r--   0        0        0    13827 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/locale/django.pot
+-rw-r--r--   0        0        0    14234 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    19878 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    22317 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14204 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    13971 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    13964 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    11650 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    21687 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    17350 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    23021 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    10750 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    23759 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14269 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    12854 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/migrations/0001_initial.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/migrations/0002_webhook_is_embed_description_change.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/migrations/0003_fleetdoctrine_link.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/migrations/0004_auto_20200915_1617.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/migrations/0005_fleettype_restricted_to_group.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/migrations/0006_fleetdoctrine_restricted_to_group.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/migrations/0007_mysql8_default_value_fixes_20201003_1232.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/migrations/0008_auto_20210114_1733.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/migrations/0009_remove_webhook_is_embedded_remove_webhook_type_and_more.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/migrations/0010_use_ellipsis_character_in_strings.py
+-rw-r--r--   0        0        0    12638 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/migrations/0011_settings_and_verbose_names.py
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/migrations/0012_migrate_app_settings_from_local_py_to_database.py
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/migrations/0013_fleetcomm_channel.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/migrations/0014_update_models.py
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/migrations/0015_alter_discordpingtarget_options_and_more.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/migrations/__init__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/static/fleetpings/css/fleetpings.css
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/static/fleetpings/css/fleetpings.min.css
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/static/fleetpings/css/fleetpings.min.css.map
+-rw-r--r--   0        0        0    15722 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/static/fleetpings/js/fleetpings.js
+-rw-r--r--   0        0        0     5551 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/static/fleetpings/js/fleetpings.min.js
+-rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/static/fleetpings/js/fleetpings.min.js.map
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/static/fleetpings/libs/flexdatalist/2.3.0/LICENSE
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/static/fleetpings/libs/flexdatalist/2.3.0/README.md
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/static/fleetpings/libs/flexdatalist/2.3.0/jquery.flexdatalist.css
+-rw-r--r--   0        0        0    77378 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/static/fleetpings/libs/flexdatalist/2.3.0/jquery.flexdatalist.js
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/static/fleetpings/libs/flexdatalist/2.3.0/jquery.flexdatalist.min.css
+-rw-r--r--   0        0        0    24873 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/static/fleetpings/libs/flexdatalist/2.3.0/jquery.flexdatalist.min.js
+-rw-r--r--   0        0        0    23171 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/static/fleetpings/libs/flexdatalist/2.3.0/jquery.flexdatalist.min.js.map
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/base.html
+-rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/index.html
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/bundles/fleetpings-css.html
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/bundles/fleetpings-js.html
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/bundles/flexdatalist-css.html
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/bundles/flexdatalist-js.html
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/partials/form/form.html
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/partials/form/segments/fleet-comms.html
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/partials/form/segments/fleet-doctrine.html
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/partials/form/segments/fleet-formup-location.html
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/partials/form/segments/fleet-type-loop.html
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/partials/form/segments/fleet-type.html
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/partials/form/segments/ping-channel.html
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/partials/form/segments/ping-targets-loop.html
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/partials/form/segments/ping-targets.html
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/partials/header/page-header.html
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/partials/ping/copy-paste-text.html
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/partials/ping/ping.html
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/templatetags/__init__.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/templatetags/fleetpings.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/tests/__init__.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/tests/test_access.py
+-rw-r--r--   0        0        0    12747 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/tests/test_ajax_calls.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/tests/test_helper_eve_images.py
+-rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/tests/test_installed_modules.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/tests/test_model_discprdpingtarget.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/tests/test_model_fleetcomm.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/tests/test_model_fleetdoctrine.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/tests/test_model_fleettype.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/tests/test_model_formuplocation.py
+-rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/tests/test_model_setting.py
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/tests/test_model_webhook.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/tests/test_templatetags.py
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/fleetpings/tests/utils.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/LICENSE
+-rw-r--r--   0        0        0     8564 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/README.md
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0    51216 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.0b1/PKG-INFO
```

### Comparing `aa_fleetpings-3.0.0/fleetpings/admin.py` & `aa_fleetpings-3.0.0b1/fleetpings/admin.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/app_settings.py` & `aa_fleetpings-3.0.0b1/fleetpings/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/auth_hooks.py` & `aa_fleetpings-3.0.0b1/fleetpings/auth_hooks.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         Constructor
         """
 
         # Setup menu entry for sidebar
         MenuItemHook.__init__(
             self,
             text=__title__,
-            classes="fa-regular fa-bell",
+            classes="far fa-bell",
             url_name="fleetpings:index",
             navactive=["fleetpings:index"],
         )
 
     def render(self, request):
         """
         Render the menu item
```

### Comparing `aa_fleetpings-3.0.0/fleetpings/form.py` & `aa_fleetpings-3.0.0b1/fleetpings/form.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/managers.py` & `aa_fleetpings-3.0.0b1/fleetpings/managers.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/models.py` & `aa_fleetpings-3.0.0b1/fleetpings/models.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/urls.py` & `aa_fleetpings-3.0.0b1/fleetpings/urls.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/views.py` & `aa_fleetpings-3.0.0b1/fleetpings/views.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/helper/discord_webhook.py` & `aa_fleetpings-3.0.0b1/fleetpings/helper/discord_webhook.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/helper/eve_images.py` & `aa_fleetpings-3.0.0b1/fleetpings/helper/eve_images.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/helper/ping_context.py` & `aa_fleetpings-3.0.0b1/fleetpings/helper/ping_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,15 +189,14 @@
                     f" ([Time Zone Conversion]({timezones_url}))"
                 )
 
             # Add local time
             webhook_ping_text_content += (
                 "\n**Formup (Local Time):** "
                 f'<t:{ping_context["formup_time"]["timestamp"]}:F>'
-                f' (<t:{ping_context["formup_time"]["timestamp"]}:R>)'
             )
     # Check if fleet comms is available
     if ping_context["fleet_comms"]:
         webhook_ping_text_content += f'\n**Comms:** {ping_context["fleet_comms"]}'
 
     # Check if doctrine is available
     if ping_context["doctrine"]["name"]:
```

### Comparing `aa_fleetpings-3.0.0/fleetpings/locale/django.pot` & `aa_fleetpings-3.0.0b1/fleetpings/locale/django.pot`

 * *Files 2% similar despite different names*

```diff
@@ -4,454 +4,454 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-15 21:21+0100\n"
+"POT-Creation-Date: 2023-10-01 17:17+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: fleetpings/__init__.py:10 fleetpings/templates/fleetpings/base.html:6
+#: fleetpings/__init__.py:12 fleetpings/templates/fleetpings/base.html:5
 #: fleetpings/templates/fleetpings/base.html:10
 msgid "Fleet Pings"
 msgstr ""
 
-#: fleetpings/admin.py:114 fleetpings/models.py:167
+#: fleetpings/admin.py:104 fleetpings/models.py:147
 msgid "Fleet comm"
 msgstr ""
 
-#: fleetpings/admin.py:144 fleetpings/form.py:151
+#: fleetpings/admin.py:125 fleetpings/form.py:149
 msgid "Doctrine"
 msgstr ""
 
-#: fleetpings/admin.py:158 fleetpings/form.py:158 fleetpings/models.py:192
+#: fleetpings/admin.py:130 fleetpings/form.py:156 fleetpings/models.py:172
 msgid "Doctrine link"
 msgstr ""
 
-#: fleetpings/admin.py:173 fleetpings/admin.py:244 fleetpings/admin.py:325
-#: fleetpings/admin.py:370 fleetpings/models.py:201 fleetpings/models.py:344
-#: fleetpings/models.py:451 fleetpings/models.py:522
+#: fleetpings/admin.py:136 fleetpings/admin.py:189 fleetpings/admin.py:243
+#: fleetpings/admin.py:288 fleetpings/models.py:181 fleetpings/models.py:308
+#: fleetpings/models.py:395 fleetpings/models.py:459
 msgid "Group restrictions"
 msgstr ""
 
-#: fleetpings/admin.py:229 fleetpings/form.py:76
+#: fleetpings/admin.py:183 fleetpings/form.py:74
 msgid "Ping target"
 msgstr ""
 
-#: fleetpings/admin.py:289 fleetpings/form.py:93 fleetpings/models.py:485
+#: fleetpings/admin.py:225 fleetpings/form.py:91 fleetpings/models.py:422
 msgid "Fleet type"
 msgstr ""
 
-#: fleetpings/admin.py:303 fleetpings/models.py:442
+#: fleetpings/admin.py:230 fleetpings/models.py:386
 msgid "Embed color"
 msgstr ""
 
-#: fleetpings/admin.py:359 fleetpings/models.py:500
+#: fleetpings/admin.py:277 fleetpings/models.py:437
 msgid "Discord channel"
 msgstr ""
 
-#: fleetpings/admin.py:364 fleetpings/models.py:513
+#: fleetpings/admin.py:282 fleetpings/models.py:450
 msgid "Webhook URL"
 msgstr ""
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: fleetpings/apps.py:21
 #, python-brace-format
 msgid "Fleet Pings v{__version__}"
 msgstr ""
 
-#: fleetpings/form.py:27
+#: fleetpings/form.py:25
 msgid "Discord Markdown"
 msgstr ""
 
-#: fleetpings/form.py:34
+#: fleetpings/form.py:32
 #, python-brace-format
 msgid "Hint: You can use {discord_markdown_link} to format the text."
 msgstr ""
 
-#: fleetpings/form.py:78
+#: fleetpings/form.py:76
 msgid "Who do you want to ping?"
 msgstr ""
 
-#: fleetpings/form.py:83
+#: fleetpings/form.py:81
 msgid "Pre-Ping"
 msgstr ""
 
-#: fleetpings/form.py:84
+#: fleetpings/form.py:82
 msgid "Mark this checkbox if this should be a pre-ping."
 msgstr ""
 
-#: fleetpings/form.py:88
+#: fleetpings/form.py:86
 msgid "Ping to"
 msgstr ""
 
-#: fleetpings/form.py:90
+#: fleetpings/form.py:88
 msgid "Select a channel to ping automatically."
 msgstr ""
 
-#: fleetpings/form.py:97
+#: fleetpings/form.py:95
 msgid "FC name"
 msgstr ""
 
-#: fleetpings/form.py:99
+#: fleetpings/form.py:97
 msgid "Who is the FC?"
 msgstr ""
 
-#: fleetpings/form.py:103
+#: fleetpings/form.py:101
 msgid "Fleet name"
 msgstr ""
 
-#: fleetpings/form.py:107
+#: fleetpings/form.py:105
 msgid "What is the fleet name in the fleet finder in Eve?"
 msgstr ""
 
-#: fleetpings/form.py:113 fleetpings/models.py:305
+#: fleetpings/form.py:111 fleetpings/models.py:269
 msgid "Formup location"
 msgstr ""
 
-#: fleetpings/form.py:120
+#: fleetpings/form.py:118
 msgid "Formup time"
 msgstr ""
 
-#: fleetpings/form.py:124
+#: fleetpings/form.py:122
 msgid ""
 "To enable this field, either make it a pre-ping (checkbox above) or uncheck "
 "\"Formup NOW\" (checkbox below)."
 msgstr ""
 
-#: fleetpings/form.py:130
+#: fleetpings/form.py:128
 msgid "Formup timestamp"
 msgstr ""
 
-#: fleetpings/form.py:136
+#: fleetpings/form.py:134
 msgid "Formup NOW"
 msgstr ""
 
-#: fleetpings/form.py:138
+#: fleetpings/form.py:136
 msgid ""
 "If this checkbox is active, formup time will be set to \"NOW\" and the time "
 "in the field above (if any is set) will be ignored."
 msgstr ""
 
-#: fleetpings/form.py:144 fleetpings/models.py:168
+#: fleetpings/form.py:142 fleetpings/models.py:148
 msgid "Fleet comms"
 msgstr ""
 
-#: fleetpings/form.py:163
+#: fleetpings/form.py:161
 msgid "Webhook embed color"
 msgstr ""
 
-#: fleetpings/form.py:169
+#: fleetpings/form.py:167
 msgid "SRP"
 msgstr ""
 
-#: fleetpings/form.py:170
+#: fleetpings/form.py:168
 msgid "Is this fleet covered by SRP?"
 msgstr ""
 
-#: fleetpings/form.py:175
+#: fleetpings/form.py:173
 msgid "Create SRP link"
 msgstr ""
 
-#: fleetpings/form.py:177
+#: fleetpings/form.py:175
 msgid ""
 "If this checkbox is active, a SRP link specific for this fleet will be "
 "created.<br>Leave blank if unsure."
 msgstr ""
 
-#: fleetpings/form.py:183
+#: fleetpings/form.py:181
 msgid "Additional information"
 msgstr ""
 
-#: fleetpings/form.py:190
+#: fleetpings/form.py:188
 msgid "Feel free to add some more information about the fleet …"
 msgstr ""
 
-#: fleetpings/form.py:199
+#: fleetpings/form.py:197
 msgid "Create Optimer"
 msgstr ""
 
-#: fleetpings/form.py:201
+#: fleetpings/form.py:199
 msgid ""
 "If this checkbox is active, a fleet operations timer for this pre-ping will "
 "be created."
 msgstr ""
 
-#: fleetpings/models.py:41
+#: fleetpings/models.py:40
 msgid "You might want to install the Discord service first …"
 msgstr ""
 
-#: fleetpings/models.py:49
+#: fleetpings/models.py:47
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
 
-#: fleetpings/models.py:55
+#: fleetpings/models.py:51
 msgid "This group has not been synced to Discord yet."
 msgstr ""
 
-#: fleetpings/models.py:117
+#: fleetpings/models.py:104
 msgid "Can access this app"
 msgstr ""
 
-#: fleetpings/models.py:127
+#: fleetpings/models.py:114
 msgid "Short name to identify this comms"
 msgstr ""
 
-#: fleetpings/models.py:128 fleetpings/models.py:184 fleetpings/models.py:272
-#: fleetpings/models.py:434
+#: fleetpings/models.py:115 fleetpings/models.py:164 fleetpings/models.py:242
+#: fleetpings/models.py:378
 msgid "Name"
 msgstr ""
 
-#: fleetpings/models.py:134
+#: fleetpings/models.py:121
 msgid "In which channel is the fleet?"
 msgstr ""
 
-#: fleetpings/models.py:135
+#: fleetpings/models.py:122
 msgid "Channel"
 msgstr ""
 
-#: fleetpings/models.py:141 fleetpings/models.py:208 fleetpings/models.py:279
-#: fleetpings/models.py:351 fleetpings/models.py:458
+#: fleetpings/models.py:128 fleetpings/models.py:188 fleetpings/models.py:249
+#: fleetpings/models.py:315 fleetpings/models.py:402
 msgid "You can add notes about this configuration here if you want"
 msgstr ""
 
-#: fleetpings/models.py:142 fleetpings/models.py:209 fleetpings/models.py:280
-#: fleetpings/models.py:352 fleetpings/models.py:459 fleetpings/models.py:530
+#: fleetpings/models.py:129 fleetpings/models.py:189 fleetpings/models.py:250
+#: fleetpings/models.py:316 fleetpings/models.py:403 fleetpings/models.py:467
 msgid "Notes"
 msgstr ""
 
-#: fleetpings/models.py:148
+#: fleetpings/models.py:135
 msgid "Whether this comms is enabled or not"
 msgstr ""
 
-#: fleetpings/models.py:149 fleetpings/models.py:217 fleetpings/models.py:288
-#: fleetpings/models.py:360 fleetpings/models.py:467 fleetpings/models.py:538
+#: fleetpings/models.py:136 fleetpings/models.py:197 fleetpings/models.py:258
+#: fleetpings/models.py:324 fleetpings/models.py:411 fleetpings/models.py:475
 msgid "Is enabled"
 msgstr ""
 
-#: fleetpings/models.py:183
+#: fleetpings/models.py:163
 msgid "Short name to identify this doctrine"
 msgstr ""
 
-#: fleetpings/models.py:191
+#: fleetpings/models.py:171
 msgid "A link to a doctrine page for this doctrine if you have."
 msgstr ""
 
-#: fleetpings/models.py:200
+#: fleetpings/models.py:180
 msgid "Restrict this doctrine to the following groups …"
 msgstr ""
 
-#: fleetpings/models.py:216
+#: fleetpings/models.py:196
 msgid "Whether this doctrine is enabled or not"
 msgstr ""
 
-#: fleetpings/models.py:237
+#: fleetpings/models.py:214
 msgid "Your doctrine URL is not valid."
 msgstr ""
 
-#: fleetpings/models.py:257
+#: fleetpings/models.py:227
 msgid "Fleet doctrine"
 msgstr ""
 
-#: fleetpings/models.py:258
+#: fleetpings/models.py:228
 msgid "Fleet doctrines"
 msgstr ""
 
-#: fleetpings/models.py:271
+#: fleetpings/models.py:241
 msgid "Short name to identify this formup location"
 msgstr ""
 
-#: fleetpings/models.py:287 fleetpings/models.py:359
+#: fleetpings/models.py:257 fleetpings/models.py:323
 msgid "Whether this formup location is enabled or not"
 msgstr ""
 
-#: fleetpings/models.py:306
+#: fleetpings/models.py:270
 msgid "Formup locations"
 msgstr ""
 
-#: fleetpings/models.py:322
+#: fleetpings/models.py:286
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 
-#: fleetpings/models.py:326
+#: fleetpings/models.py:290
 msgid "Group name"
 msgstr ""
 
-#: fleetpings/models.py:334
+#: fleetpings/models.py:298
 msgid "ID of the Discord role to ping"
 msgstr ""
 
-#: fleetpings/models.py:335
+#: fleetpings/models.py:299
 msgid "Discord ID"
 msgstr ""
 
-#: fleetpings/models.py:343 fleetpings/models.py:521
+#: fleetpings/models.py:307 fleetpings/models.py:458
 msgid "Restrict ping rights to the following groups …"
 msgstr ""
 
-#: fleetpings/models.py:419
+#: fleetpings/models.py:363
 msgid "Discord ping target"
 msgstr ""
 
-#: fleetpings/models.py:420
+#: fleetpings/models.py:364
 msgid "Discord ping targets"
 msgstr ""
 
-#: fleetpings/models.py:433
+#: fleetpings/models.py:377
 msgid "Short name to identify this fleet type"
 msgstr ""
 
-#: fleetpings/models.py:441
+#: fleetpings/models.py:385
 msgid "Highlight color for the embed"
 msgstr ""
 
-#: fleetpings/models.py:450
+#: fleetpings/models.py:394
 msgid "Restrict this fleet type to the following groups …"
 msgstr ""
 
-#: fleetpings/models.py:466
+#: fleetpings/models.py:410
 msgid "Whether this fleet type is enabled or not"
 msgstr ""
 
-#: fleetpings/models.py:486
+#: fleetpings/models.py:423
 msgid "Fleet types"
 msgstr ""
 
-#: fleetpings/models.py:499
+#: fleetpings/models.py:436
 msgid "Name of the channel this webhook posts to"
 msgstr ""
 
-#: fleetpings/models.py:509
+#: fleetpings/models.py:446
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
 
-#: fleetpings/models.py:529
+#: fleetpings/models.py:466
 msgid "You can add notes about this webhook here if you want"
 msgstr ""
 
-#: fleetpings/models.py:537
+#: fleetpings/models.py:474
 msgid "Whether this webhook is active or not"
 msgstr ""
 
-#: fleetpings/models.py:556
+#: fleetpings/models.py:486
 msgid "Webhook"
 msgstr ""
 
-#: fleetpings/models.py:557
+#: fleetpings/models.py:487
 msgid "Webhooks"
 msgstr ""
 
-#: fleetpings/models.py:576
+#: fleetpings/models.py:502
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 
-#: fleetpings/models.py:596
+#: fleetpings/models.py:522
 msgid "Use default fleet types"
 msgstr ""
 
-#: fleetpings/models.py:599
+#: fleetpings/models.py:525
 msgid "Use default ping targets"
 msgstr ""
 
-#: fleetpings/models.py:602
+#: fleetpings/models.py:528
 msgid "Use Doctrines from Fittings module"
 msgstr ""
 
-#: fleetpings/models.py:604
+#: fleetpings/models.py:530
 msgid "Verify webhooks"
 msgstr ""
 
-#: fleetpings/models.py:605
+#: fleetpings/models.py:531
 msgid "Default embed color"
 msgstr ""
 
-#: fleetpings/models.py:611
+#: fleetpings/models.py:537
 msgid ""
 "Whether to use default fleet types. If checked, the default fleet types "
 "(Roaming, Home Defense, StratOP, and CTA) will be added to the Fleet Type "
 "dropdown."
 msgstr ""
 
-#: fleetpings/models.py:622
+#: fleetpings/models.py:548
 msgid ""
 "Whether to use default ping targets. If checked, the default ping targets "
 "(@everyone and @here) will be added to the Ping Target dropdown."
 msgstr ""
 
-#: fleetpings/models.py:632
+#: fleetpings/models.py:558
 msgid ""
 "Whether to use the doctrines from the Fittings modules in the doctrine "
 "dropdown. Note: The fittings module needs to be installed for this."
 msgstr ""
 
-#: fleetpings/models.py:642
+#: fleetpings/models.py:568
 msgid ""
 "Whether to verify webhooks URLs or not. Note: When unchecked, webhook URLs "
 "will not be verified, so the app can be used with non-Discord webhooks as "
 "well. When disabling webhook verification and using non-Discord webhooks, it "
 "is up to you to make sure your webhook understands a payload that is "
 "formatted for Discord webhooks."
 msgstr ""
 
-#: fleetpings/models.py:655
+#: fleetpings/models.py:581
 msgid "Default highlight color for the webhook embed."
 msgstr ""
 
-#: fleetpings/models.py:667
+#: fleetpings/models.py:593
 msgid "Setting"
 msgstr ""
 
-#: fleetpings/models.py:668
+#: fleetpings/models.py:594
 msgid "Settings"
 msgstr ""
 
-#: fleetpings/models.py:678
+#: fleetpings/models.py:597
 msgid "Fleet Pings Settings"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/index.html:11
 msgid "Fleet information"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/index.html:23
+#: fleetpings/templates/fleetpings/index.html:22
 msgid "Formatted ping text"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/index.html:51
+#: fleetpings/templates/fleetpings/index.html:49
 msgid ""
 "Mandatory information is missing. To create an optimer, you need to provide "
 "all of the following information:<br>» FC name<br>» Fleet name<br>» Formup "
 "location<br>» Formup time<br>» Ships / Doctrine"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/index.html:56
+#: fleetpings/templates/fleetpings/index.html:54
 msgid ""
 "Mandatory information is missing. To create an SRP link, you need to provide "
 "all of the following information:<br>» Fleet name<br>» Ships / Doctrine"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/index.html:60
+#: fleetpings/templates/fleetpings/index.html:58
 msgid ""
 "Error! Your ping was not copied to your clipboard. Maybe your browser "
 "doesn&apos;t support this feature."
 msgstr ""
 
-#: fleetpings/templates/fleetpings/index.html:61
+#: fleetpings/templates/fleetpings/index.html:59
 msgid ""
 "Success! Your ping text has been copied to your clipboard. Now be a good FC "
 "and throw it in your chat so you actually get some people in fleet."
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:5
 msgid ""
@@ -459,42 +459,42 @@
 "existing translation?"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/form.html:69
+#: fleetpings/templates/fleetpings/partials/form/form.html:68
 msgid "Create ping"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:6
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:7
 msgid "Please think twice if you really need to ping <code>@everyone</code>."
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:10
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:11
 msgid ""
 "\n"
-"                <code>@everyone</code>\n"
-"                includes also all the people in this channel who are offline "
-"and\n"
-"                possibly asleep at the moment and might be waking up when "
-"their\n"
-"                mobile devices ping. Or they wake up hours later to "
+"                    <code>@everyone</code>\n"
+"                    includes also all the people in this channel who are "
+"offline and\n"
+"                    possibly asleep at the moment and might be waking up "
+"when their\n"
+"                    mobile devices ping. Or they wake up hours later to "
 "irrelevant\n"
-"                pings by the time they open Discord.\n"
-"            "
+"                    pings by the time they open Discord.\n"
+"                "
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:20
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:21
 msgid ""
 "Notification spam is a real thing and might entice people to mute channels."
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:24
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:25
 msgid "<code>@here</code> usually does the trick just fine."
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/form/segments/fleet-type.html:3
 msgid "Please select"
 msgstr ""
 
@@ -534,26 +534,26 @@
 msgid "No ping created yet …"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/ping/ping.html:22
 msgid "Copy ping text"
 msgstr ""
 
-#: fleetpings/views.py:439
+#: fleetpings/views.py:394
 msgid "Not all mandatory information available to create an SRP link."
 msgstr ""
 
-#: fleetpings/views.py:474
+#: fleetpings/views.py:426
 msgid "Fleet operations timer has been created …"
 msgstr ""
 
-#: fleetpings/views.py:483
+#: fleetpings/views.py:435
 msgid "SRP link has been created …"
 msgstr ""
 
-#: fleetpings/views.py:500
+#: fleetpings/views.py:452
 msgid "Form invalid. Please check your input."
 msgstr ""
 
-#: fleetpings/views.py:502
+#: fleetpings/views.py:454
 msgid "No form data submitted."
 msgstr ""
```

### Comparing `aa_fleetpings-3.0.0/fleetpings/locale/de/LC_MESSAGES/django.mo` & `aa_fleetpings-3.0.0b1/fleetpings/locale/de/LC_MESSAGES/django.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,38 +7,38 @@
 "Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-fleetpings/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.4.2\n"
+"X-Generator: Weblate 5.0.2\n"
 
 msgid ""
 "\n"
-"                <code>@everyone</code>\n"
-"                includes also all the people in this channel who are offline "
-"and\n"
-"                possibly asleep at the moment and might be waking up when "
-"their\n"
-"                mobile devices ping. Or they wake up hours later to "
+"                    <code>@everyone</code>\n"
+"                    includes also all the people in this channel who are "
+"offline and\n"
+"                    possibly asleep at the moment and might be waking up "
+"when their\n"
+"                    mobile devices ping. Or they wake up hours later to "
 "irrelevant\n"
-"                pings by the time they open Discord.\n"
-"            "
+"                    pings by the time they open Discord.\n"
+"                "
 msgstr ""
 "\n"
-"                <code>@everyone</code>\n"
-"                umfasst auch alle Personen in diesem Kanal, die offline sind "
-"und\n"
-"                eventuell gerade schlafen und möglicherweise aufgeweckt "
+"                    <code>@everyone</code>\n"
+"                     umfasst auch alle Personen in diesem Kanal, die offline "
+"sind und\n"
+"                     eventuell gerade schlafen und möglicherweise aufgeweckt "
 "werden, wenn ihre\n"
-"                Mobilgeräte pingen. Oder sie wachen Stunden später auf zu "
-"irrelevanten\n"
-"                Pings, wenn sie Discord öffnen.\n"
-"            "
+"                     Mobilgeräte pingen. Oder sie wachen Stunden später auf "
+"zu irrelevanten\n"
+"                     Pings, wenn sie Discord öffnen.\n"
+"                "
 
 msgid "<code>@here</code> usually does the trick just fine."
 msgstr "<code>@here</code> ist im Normalfall absolut ausreichend."
 
 msgid "A link to a doctrine page for this doctrine if you have."
 msgstr "Ein Link zu einer Doktrinenseite für diese Doktrin, falls vorhanden."
```

### Comparing `aa_fleetpings-3.0.0/fleetpings/locale/de/LC_MESSAGES/django.po` & `aa_fleetpings-3.0.0b1/fleetpings/locale/de/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,499 +1,498 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
+# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-15 21:21+0100\n"
-"PO-Revision-Date: 2024-03-16 09:25+0000\n"
+"POT-Creation-Date: 2023-10-01 17:17+0200\n"
+"PO-Revision-Date: 2023-10-02 09:47+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
 "Language-Team: German <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-fleetpings/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.4.2\n"
+"X-Generator: Weblate 5.0.2\n"
 
-#: fleetpings/__init__.py:10 fleetpings/templates/fleetpings/base.html:6
+#: fleetpings/__init__.py:12 fleetpings/templates/fleetpings/base.html:5
 #: fleetpings/templates/fleetpings/base.html:10
 msgid "Fleet Pings"
 msgstr "Flotten-Ankündigungen"
 
-#: fleetpings/admin.py:114 fleetpings/models.py:167
+#: fleetpings/admin.py:104 fleetpings/models.py:147
 msgid "Fleet comm"
 msgstr "Flottenkommunikation"
 
-#: fleetpings/admin.py:144 fleetpings/form.py:151
+#: fleetpings/admin.py:125 fleetpings/form.py:149
 msgid "Doctrine"
 msgstr "Doktrin"
 
-#: fleetpings/admin.py:158 fleetpings/form.py:158 fleetpings/models.py:192
+#: fleetpings/admin.py:130 fleetpings/form.py:156 fleetpings/models.py:172
 msgid "Doctrine link"
 msgstr "Doktrin Link"
 
-#: fleetpings/admin.py:173 fleetpings/admin.py:244 fleetpings/admin.py:325
-#: fleetpings/admin.py:370 fleetpings/models.py:201 fleetpings/models.py:344
-#: fleetpings/models.py:451 fleetpings/models.py:522
+#: fleetpings/admin.py:136 fleetpings/admin.py:189 fleetpings/admin.py:243
+#: fleetpings/admin.py:288 fleetpings/models.py:181 fleetpings/models.py:308
+#: fleetpings/models.py:395 fleetpings/models.py:459
 msgid "Group restrictions"
 msgstr "Gruppenbeschränkungen"
 
-#: fleetpings/admin.py:229 fleetpings/form.py:76
+#: fleetpings/admin.py:183 fleetpings/form.py:74
 msgid "Ping target"
 msgstr "Pingziel"
 
-#: fleetpings/admin.py:289 fleetpings/form.py:93 fleetpings/models.py:485
+#: fleetpings/admin.py:225 fleetpings/form.py:91 fleetpings/models.py:422
 msgid "Fleet type"
 msgstr "Flottenart"
 
-#: fleetpings/admin.py:303 fleetpings/models.py:442
+#: fleetpings/admin.py:230 fleetpings/models.py:386
 msgid "Embed color"
 msgstr "Embed Farbe"
 
-#: fleetpings/admin.py:359 fleetpings/models.py:500
+#: fleetpings/admin.py:277 fleetpings/models.py:437
 msgid "Discord channel"
 msgstr "Discord-Kanal"
 
-#: fleetpings/admin.py:364 fleetpings/models.py:513
+#: fleetpings/admin.py:282 fleetpings/models.py:450
 msgid "Webhook URL"
 msgstr "Webhook URL"
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: fleetpings/apps.py:21
 #, python-brace-format
 msgid "Fleet Pings v{__version__}"
 msgstr "Fleet Pings v{__version__}"
 
-#: fleetpings/form.py:27
+#: fleetpings/form.py:25
 msgid "Discord Markdown"
 msgstr "Discord Markdown"
 
-#: fleetpings/form.py:34
+#: fleetpings/form.py:32
 #, python-brace-format
 msgid "Hint: You can use {discord_markdown_link} to format the text."
 msgstr ""
 "Hinweis: Du kannst {discord_markdown_link} nutzen um den Text zu formatieren."
 
-#: fleetpings/form.py:78
+#: fleetpings/form.py:76
 msgid "Who do you want to ping?"
 msgstr "Wen möchtest Du pingen?"
 
-#: fleetpings/form.py:83
+#: fleetpings/form.py:81
 msgid "Pre-Ping"
 msgstr "Pre-Ping"
 
-#: fleetpings/form.py:84
+#: fleetpings/form.py:82
 msgid "Mark this checkbox if this should be a pre-ping."
 msgstr "Markiere dieses Kontrollkästchen, wenn dies ein Pre-Ping sein soll."
 
-#: fleetpings/form.py:88
+#: fleetpings/form.py:86
 msgid "Ping to"
 msgstr "Ping in"
 
-#: fleetpings/form.py:90
+#: fleetpings/form.py:88
 msgid "Select a channel to ping automatically."
 msgstr "Wähle einen Kanal aus, der automatisch gepingt werden soll."
 
-#: fleetpings/form.py:97
+#: fleetpings/form.py:95
 msgid "FC name"
 msgstr "FC Name"
 
-#: fleetpings/form.py:99
+#: fleetpings/form.py:97
 msgid "Who is the FC?"
 msgstr "Wer ist der FC?"
 
-#: fleetpings/form.py:103
+#: fleetpings/form.py:101
 msgid "Fleet name"
 msgstr "Flottenname"
 
-#: fleetpings/form.py:107
+#: fleetpings/form.py:105
 msgid "What is the fleet name in the fleet finder in Eve?"
 msgstr "Was ist der Name der Flotte im Flottenfinder in Eve?"
 
-#: fleetpings/form.py:113 fleetpings/models.py:305
+#: fleetpings/form.py:111 fleetpings/models.py:269
 msgid "Formup location"
 msgstr "Treffpunkt"
 
-#: fleetpings/form.py:120
+#: fleetpings/form.py:118
 msgid "Formup time"
 msgstr "Flottenstart"
 
-#: fleetpings/form.py:124
+#: fleetpings/form.py:122
 msgid ""
 "To enable this field, either make it a pre-ping (checkbox above) or uncheck "
 "\"Formup NOW\" (checkbox below)."
 msgstr ""
-"Um dieses Feld zu aktivieren, mach es entweder zu einem Pre-Ping "
-"(Kontrollkästchen oben) oder deaktiviere „Flottenstart "
-"JETZT“ (Kontrollkästchen unten)."
+"Um dieses Feld zu aktivieren, mach es entweder zu einem Pre-Ping ("
+"Kontrollkästchen oben) oder deaktiviere „Flottenstart JETZT“ ("
+"Kontrollkästchen unten)."
 
-#: fleetpings/form.py:130
+#: fleetpings/form.py:128
 msgid "Formup timestamp"
 msgstr "Flottenstart Zeitstempel"
 
-#: fleetpings/form.py:136
+#: fleetpings/form.py:134
 msgid "Formup NOW"
 msgstr "Flottenstart JETZT"
 
-#: fleetpings/form.py:138
+#: fleetpings/form.py:136
 msgid ""
 "If this checkbox is active, formup time will be set to \"NOW\" and the time "
 "in the field above (if any is set) will be ignored."
 msgstr ""
-"Wenn dieses Kontrollkästchen aktiviert ist, wird der Flottenstart auf "
-"„JETZT“ gesetzt. und die Zeit im obigen Feld (falls vorhanden) wird "
-"ignoriert."
+"Wenn dieses Kontrollkästchen aktiviert ist, wird der Flottenstart auf „JETZT“"
+" gesetzt. und die Zeit im obigen Feld (falls vorhanden) wird ignoriert."
 
-#: fleetpings/form.py:144 fleetpings/models.py:168
+#: fleetpings/form.py:142 fleetpings/models.py:148
 msgid "Fleet comms"
 msgstr "Flottenkommunikationen"
 
-#: fleetpings/form.py:163
+#: fleetpings/form.py:161
 msgid "Webhook embed color"
 msgstr "Webhook Embed-Farbe"
 
-#: fleetpings/form.py:169
+#: fleetpings/form.py:167
 msgid "SRP"
 msgstr "SRP"
 
-#: fleetpings/form.py:170
+#: fleetpings/form.py:168
 msgid "Is this fleet covered by SRP?"
 msgstr "Ist diese Flotte durch SRP abgedeckt?"
 
-#: fleetpings/form.py:175
+#: fleetpings/form.py:173
 msgid "Create SRP link"
 msgstr "SRP-Link erstellen"
 
-#: fleetpings/form.py:177
+#: fleetpings/form.py:175
 msgid ""
 "If this checkbox is active, a SRP link specific for this fleet will be "
 "created.<br>Leave blank if unsure."
 msgstr ""
 "Wenn dieses Kontrollkästchen aktiviert ist, wird ein für diese Flotte "
 "spezifischer SRP-Link erstellt.<br>Leer lassen, wenn Du Dir nicht sicher "
 "bist."
 
-#: fleetpings/form.py:183
+#: fleetpings/form.py:181
 msgid "Additional information"
 msgstr "Zusätzliche Informationen"
 
-#: fleetpings/form.py:190
+#: fleetpings/form.py:188
 msgid "Feel free to add some more information about the fleet …"
 msgstr "Fühl Dich frei, weitere Informationen über die Flotte hinzuzufügen …"
 
-#: fleetpings/form.py:199
+#: fleetpings/form.py:197
 msgid "Create Optimer"
 msgstr "Op Timer erstellen"
 
-#: fleetpings/form.py:201
+#: fleetpings/form.py:199
 msgid ""
 "If this checkbox is active, a fleet operations timer for this pre-ping will "
 "be created."
 msgstr ""
 "Wenn dieses Kontrollkästchen aktiviert ist, wird ein Op Timer für diesen Pre-"
 "Ping erstellt."
 
-#: fleetpings/models.py:41
+#: fleetpings/models.py:40
 msgid "You might want to install the Discord service first …"
 msgstr "Du solltest zunächst den Discord Service installieren …"
 
-#: fleetpings/models.py:49
+#: fleetpings/models.py:47
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
 "Bist Du sicher das Du Deinen Discord Server mit Alliance Auth verbunden hast?"
 
-#: fleetpings/models.py:55
+#: fleetpings/models.py:51
 msgid "This group has not been synced to Discord yet."
 msgstr "Diese Gruppe wurde bisher noch nicht zu Discord synchronisiert."
 
-#: fleetpings/models.py:117
+#: fleetpings/models.py:104
 msgid "Can access this app"
 msgstr "Kann auf diese App zugreifen"
 
-#: fleetpings/models.py:127
+#: fleetpings/models.py:114
 msgid "Short name to identify this comms"
 msgstr "Kurzname zur Identifizierung"
 
-#: fleetpings/models.py:128 fleetpings/models.py:184 fleetpings/models.py:272
-#: fleetpings/models.py:434
+#: fleetpings/models.py:115 fleetpings/models.py:164 fleetpings/models.py:242
+#: fleetpings/models.py:378
 msgid "Name"
 msgstr "Name"
 
-#: fleetpings/models.py:134
+#: fleetpings/models.py:121
 msgid "In which channel is the fleet?"
 msgstr "In welchem Kanal ist die Flotte?"
 
-#: fleetpings/models.py:135
+#: fleetpings/models.py:122
 msgid "Channel"
 msgstr "Kanal"
 
-#: fleetpings/models.py:141 fleetpings/models.py:208 fleetpings/models.py:279
-#: fleetpings/models.py:351 fleetpings/models.py:458
+#: fleetpings/models.py:128 fleetpings/models.py:188 fleetpings/models.py:249
+#: fleetpings/models.py:315 fleetpings/models.py:402
 msgid "You can add notes about this configuration here if you want"
 msgstr ""
 "Wenn Du möchtest, kannst Du hier Anmerkungen zu dieser Konfiguration "
 "hinzufügen"
 
-#: fleetpings/models.py:142 fleetpings/models.py:209 fleetpings/models.py:280
-#: fleetpings/models.py:352 fleetpings/models.py:459 fleetpings/models.py:530
+#: fleetpings/models.py:129 fleetpings/models.py:189 fleetpings/models.py:250
+#: fleetpings/models.py:316 fleetpings/models.py:403 fleetpings/models.py:467
 msgid "Notes"
 msgstr "Notizen"
 
-#: fleetpings/models.py:148
+#: fleetpings/models.py:135
 msgid "Whether this comms is enabled or not"
 msgstr "Ist aktiv oder nicht"
 
-#: fleetpings/models.py:149 fleetpings/models.py:217 fleetpings/models.py:288
-#: fleetpings/models.py:360 fleetpings/models.py:467 fleetpings/models.py:538
+#: fleetpings/models.py:136 fleetpings/models.py:197 fleetpings/models.py:258
+#: fleetpings/models.py:324 fleetpings/models.py:411 fleetpings/models.py:475
 msgid "Is enabled"
 msgstr "Ist aktiviert"
 
-#: fleetpings/models.py:183
+#: fleetpings/models.py:163
 msgid "Short name to identify this doctrine"
 msgstr "Kurzname der Doktrin"
 
-#: fleetpings/models.py:191
+#: fleetpings/models.py:171
 msgid "A link to a doctrine page for this doctrine if you have."
 msgstr "Ein Link zu einer Doktrinenseite für diese Doktrin, falls vorhanden."
 
-#: fleetpings/models.py:200
+#: fleetpings/models.py:180
 msgid "Restrict this doctrine to the following groups …"
 msgstr "Beschränkt diese Doktrin auf die folgenden Gruppen …"
 
-#: fleetpings/models.py:216
+#: fleetpings/models.py:196
 msgid "Whether this doctrine is enabled or not"
 msgstr "Ist diese Doktrin aktive oder nicht"
 
-#: fleetpings/models.py:237
+#: fleetpings/models.py:214
 msgid "Your doctrine URL is not valid."
 msgstr "Die Doktrin-URL ist ungültig."
 
-#: fleetpings/models.py:257
+#: fleetpings/models.py:227
 msgid "Fleet doctrine"
 msgstr "Flottendoktrin"
 
-#: fleetpings/models.py:258
+#: fleetpings/models.py:228
 msgid "Fleet doctrines"
 msgstr "Flottendoktrinen"
 
-#: fleetpings/models.py:271
+#: fleetpings/models.py:241
 msgid "Short name to identify this formup location"
 msgstr "Kurzname für den Treffpunkt"
 
-#: fleetpings/models.py:287 fleetpings/models.py:359
+#: fleetpings/models.py:257 fleetpings/models.py:323
 msgid "Whether this formup location is enabled or not"
 msgstr "Ist dieser Treffpunkt aktiv oder nicht"
 
-#: fleetpings/models.py:306
+#: fleetpings/models.py:270
 msgid "Formup locations"
 msgstr "Treffpunkte"
 
-#: fleetpings/models.py:322
+#: fleetpings/models.py:286
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 "Name der Discord Rolle zum Pingen. (Hinweis: Dies muss eine Auth Gruppe sein "
 "die zu Discord synchronisiert wurde.)"
 
-#: fleetpings/models.py:326
+#: fleetpings/models.py:290
 msgid "Group name"
 msgstr "Gruppenname"
 
-#: fleetpings/models.py:334
+#: fleetpings/models.py:298
 msgid "ID of the Discord role to ping"
 msgstr "ID der Discord Rolle zum Pingen"
 
-#: fleetpings/models.py:335
+#: fleetpings/models.py:299
 msgid "Discord ID"
 msgstr "Discord ID"
 
-#: fleetpings/models.py:343 fleetpings/models.py:521
+#: fleetpings/models.py:307 fleetpings/models.py:458
 msgid "Restrict ping rights to the following groups …"
 msgstr "Beschränkt die Ping-Rechte auf die folgenden Gruppen …"
 
-#: fleetpings/models.py:419
+#: fleetpings/models.py:363
 msgid "Discord ping target"
 msgstr "Discord Pingziel"
 
-#: fleetpings/models.py:420
+#: fleetpings/models.py:364
 msgid "Discord ping targets"
 msgstr "Discord Pingziele"
 
-#: fleetpings/models.py:433
+#: fleetpings/models.py:377
 msgid "Short name to identify this fleet type"
 msgstr "Kurzname für die Flottenart"
 
-#: fleetpings/models.py:441
+#: fleetpings/models.py:385
 msgid "Highlight color for the embed"
 msgstr "Highlight Farbe für den Embed"
 
-#: fleetpings/models.py:450
+#: fleetpings/models.py:394
 msgid "Restrict this fleet type to the following groups …"
 msgstr "Beschränkt diese Flottenart auf die folgenden Gruppen …"
 
-#: fleetpings/models.py:466
+#: fleetpings/models.py:410
 msgid "Whether this fleet type is enabled or not"
 msgstr "Ist diese Flottenart aktiv oder nicht"
 
-#: fleetpings/models.py:486
+#: fleetpings/models.py:423
 msgid "Fleet types"
 msgstr "Flottenarten"
 
-#: fleetpings/models.py:499
+#: fleetpings/models.py:436
 msgid "Name of the channel this webhook posts to"
 msgstr "Name des Kanals in dem dieser Webhook postet"
 
-#: fleetpings/models.py:509
+#: fleetpings/models.py:446
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
 "URL des Webhooks, z. B.: https://discord.com/api/webhooks/123456/abcdef"
 
-#: fleetpings/models.py:529
+#: fleetpings/models.py:466
 msgid "You can add notes about this webhook here if you want"
 msgstr ""
 "Wenn Du möchtest, kannst Du hier Anmerkungen zu diesem Webhook hinzufügen"
 
-#: fleetpings/models.py:537
+#: fleetpings/models.py:474
 msgid "Whether this webhook is active or not"
 msgstr "Ist dieser Webhook aktiv oder nicht"
 
-#: fleetpings/models.py:556
+#: fleetpings/models.py:486
 msgid "Webhook"
 msgstr "Webhook"
 
-#: fleetpings/models.py:557
+#: fleetpings/models.py:487
 msgid "Webhooks"
 msgstr "Webhooks"
 
-#: fleetpings/models.py:576
+#: fleetpings/models.py:502
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 "Ungültige Webhook-URL. Die eingegebene Webhook-URL stimmt mit keinem "
 "bekannten Format für einen Discord-Webhook überein. Bitte überprüfe die "
 "Webhook-URL."
 
-#: fleetpings/models.py:596
+#: fleetpings/models.py:522
 msgid "Use default fleet types"
 msgstr "Standard Flottenarten nutzen"
 
-#: fleetpings/models.py:599
+#: fleetpings/models.py:525
 msgid "Use default ping targets"
 msgstr "Standard Pingziele nutzen"
 
-#: fleetpings/models.py:602
+#: fleetpings/models.py:528
 msgid "Use Doctrines from Fittings module"
 msgstr "Doktrinen vom Fittings Modul nutzen"
 
-#: fleetpings/models.py:604
+#: fleetpings/models.py:530
 msgid "Verify webhooks"
 msgstr "Webhooks verifizieren"
 
-#: fleetpings/models.py:605
+#: fleetpings/models.py:531
 msgid "Default embed color"
 msgstr "Standard Embed Farbe"
 
-#: fleetpings/models.py:611
+#: fleetpings/models.py:537
 msgid ""
 "Whether to use default fleet types. If checked, the default fleet types "
 "(Roaming, Home Defense, StratOP, and CTA) will be added to the Fleet Type "
 "dropdown."
 msgstr ""
 "Nutze Standard Flottenarten. Wenn angehakt, werden die Standard Flottenarten "
 "(Roaming, Home Defense, StratOP, and CTA) dem Dropdown im Formular "
 "hinzugefügt."
 
-#: fleetpings/models.py:622
+#: fleetpings/models.py:548
 msgid ""
 "Whether to use default ping targets. If checked, the default ping targets "
 "(@everyone and @here) will be added to the Ping Target dropdown."
 msgstr ""
 "Standard Pingziele nutzen. Wenn angehakt, werden die Standard Pingziele "
 "(@everyone and @here) dem Dropdown im Formular hinzugefügt."
 
-#: fleetpings/models.py:632
+#: fleetpings/models.py:558
 msgid ""
 "Whether to use the doctrines from the Fittings modules in the doctrine "
 "dropdown. Note: The fittings module needs to be installed for this."
 msgstr ""
 "Sollen die Doktrinen aus dem Fittings Modul genutzt werden? Hinweis: das "
 "Fittings Module muss hierfür installiert sein."
 
-#: fleetpings/models.py:642
+#: fleetpings/models.py:568
 msgid ""
 "Whether to verify webhooks URLs or not. Note: When unchecked, webhook URLs "
 "will not be verified, so the app can be used with non-Discord webhooks as "
 "well. When disabling webhook verification and using non-Discord webhooks, it "
 "is up to you to make sure your webhook understands a payload that is "
 "formatted for Discord webhooks."
 msgstr ""
 "Webhook URLs prüfen. Wenn abgewählt werden die Webhook URLs nicht geprüft "
 "und es können Webhooks verwendet werden die nicht von Discord sind. Es ist "
 "Deine Verantwortung sicherzustellen dass diese Webhooks das Discord Format "
 "verstehen."
 
-#: fleetpings/models.py:655
+#: fleetpings/models.py:581
 msgid "Default highlight color for the webhook embed."
 msgstr "Standard Highlight Farbe für den Webhook Embed."
 
-#: fleetpings/models.py:667
+#: fleetpings/models.py:593
 msgid "Setting"
 msgstr "Einstellung"
 
-#: fleetpings/models.py:668
+#: fleetpings/models.py:594
 msgid "Settings"
 msgstr "Einstellungen"
 
-#: fleetpings/models.py:678
+#: fleetpings/models.py:597
 msgid "Fleet Pings Settings"
 msgstr "Fleet Pings Einstellungen"
 
 #: fleetpings/templates/fleetpings/index.html:11
 msgid "Fleet information"
 msgstr "Flotteninformation"
 
-#: fleetpings/templates/fleetpings/index.html:23
+#: fleetpings/templates/fleetpings/index.html:22
 msgid "Formatted ping text"
 msgstr "Formatierter Ankündigungstext"
 
-#: fleetpings/templates/fleetpings/index.html:51
+#: fleetpings/templates/fleetpings/index.html:49
 msgid ""
 "Mandatory information is missing. To create an optimer, you need to provide "
 "all of the following information:<br>» FC name<br>» Fleet name<br>» Formup "
 "location<br>» Formup time<br>» Ships / Doctrine"
 msgstr ""
 "Pflichtangaben fehlen. Um einen Optimierer zu erstellen, müssen alle der "
 "folgenden Informationen angegeben sein:<br>» FC-Name<br>» Flottenname<br>» "
 "Treffpunkt<br>» Flottenstart<br>» Schiffe / Doktrin"
 
-#: fleetpings/templates/fleetpings/index.html:56
+#: fleetpings/templates/fleetpings/index.html:54
 msgid ""
 "Mandatory information is missing. To create an SRP link, you need to provide "
 "all of the following information:<br>» Fleet name<br>» Ships / Doctrine"
 msgstr ""
 "Pflichtangaben fehlen. Um einen SRP-Link zu erstellen, müssen alle der "
 "folgenden Informationen angegeben sein:<br>» Flottenname<br>» Schiffe / "
 "Doktrin"
 
-#: fleetpings/templates/fleetpings/index.html:60
+#: fleetpings/templates/fleetpings/index.html:58
 msgid ""
 "Error! Your ping was not copied to your clipboard. Maybe your browser "
 "doesn&apos;t support this feature."
 msgstr ""
 "Fehler! Der Ping wurde nicht in Ihre Zwischenablage kopiert. Möglicherweise "
 "unterstützt Dein Browser diese Funktion nicht."
 
-#: fleetpings/templates/fleetpings/index.html:61
+#: fleetpings/templates/fleetpings/index.html:59
 msgid ""
 "Success! Your ping text has been copied to your clipboard. Now be a good FC "
 "and throw it in your chat so you actually get some people in fleet."
 msgstr ""
 "Erfolg! Der Ping-Text wurde in Ihre Zwischenablage kopiert. Sei jetzt ein "
 "guter FC und wirf Sie es in einen Discord Chat, damit auch einige Leute in "
 "die Flotte kommen."
@@ -506,55 +505,55 @@
 "Du möchtest helfen diese App in Deine Sprache zu übersetzen oder die "
 "bestehende Übersetzung verbessern?"
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "Tritt unserm Team von Übersetzern bei!"
 
-#: fleetpings/templates/fleetpings/partials/form/form.html:69
+#: fleetpings/templates/fleetpings/partials/form/form.html:68
 msgid "Create ping"
 msgstr "Ping erstellen"
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:6
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:7
 msgid "Please think twice if you really need to ping <code>@everyone</code>."
 msgstr ""
 "Bitte überlege zweimal, ob Du wirklich <code>@everyone</code> pingen musst."
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:10
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:11
 msgid ""
 "\n"
-"                <code>@everyone</code>\n"
-"                includes also all the people in this channel who are offline "
-"and\n"
-"                possibly asleep at the moment and might be waking up when "
-"their\n"
-"                mobile devices ping. Or they wake up hours later to "
+"                    <code>@everyone</code>\n"
+"                    includes also all the people in this channel who are "
+"offline and\n"
+"                    possibly asleep at the moment and might be waking up "
+"when their\n"
+"                    mobile devices ping. Or they wake up hours later to "
 "irrelevant\n"
-"                pings by the time they open Discord.\n"
-"            "
+"                    pings by the time they open Discord.\n"
+"                "
 msgstr ""
 "\n"
-"                <code>@everyone</code>\n"
-"                umfasst auch alle Personen in diesem Kanal, die offline sind "
-"und\n"
-"                eventuell gerade schlafen und möglicherweise aufgeweckt "
+"                    <code>@everyone</code>\n"
+"                     umfasst auch alle Personen in diesem Kanal, die offline "
+"sind und\n"
+"                     eventuell gerade schlafen und möglicherweise aufgeweckt "
 "werden, wenn ihre\n"
-"                Mobilgeräte pingen. Oder sie wachen Stunden später auf zu "
-"irrelevanten\n"
-"                Pings, wenn sie Discord öffnen.\n"
-"            "
+"                     Mobilgeräte pingen. Oder sie wachen Stunden später auf "
+"zu irrelevanten\n"
+"                     Pings, wenn sie Discord öffnen.\n"
+"                "
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:20
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:21
 msgid ""
 "Notification spam is a real thing and might entice people to mute channels."
 msgstr ""
 "Benachrichtigungs-Spam ist eine reale Sache und könnte Leute dazu verleiten, "
 "Kanäle stummzuschalten."
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:24
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:25
 msgid "<code>@here</code> usually does the trick just fine."
 msgstr "<code>@here</code> ist im Normalfall absolut ausreichend."
 
 #: fleetpings/templates/fleetpings/partials/form/segments/fleet-type.html:3
 msgid "Please select"
 msgstr "Bitte wählen"
 
@@ -594,28 +593,28 @@
 msgid "No ping created yet …"
 msgstr "Noch kein Ping erstellt …"
 
 #: fleetpings/templates/fleetpings/partials/ping/ping.html:22
 msgid "Copy ping text"
 msgstr "Ping-Text kopieren"
 
-#: fleetpings/views.py:439
+#: fleetpings/views.py:394
 msgid "Not all mandatory information available to create an SRP link."
 msgstr ""
 "Nicht alle obligatorischen Informationen zum Erstellen eines SRP-Links "
 "verfügbar."
 
-#: fleetpings/views.py:474
+#: fleetpings/views.py:426
 msgid "Fleet operations timer has been created …"
 msgstr "Der Timer für Flottenoperationen wurde erstellt …"
 
-#: fleetpings/views.py:483
+#: fleetpings/views.py:435
 msgid "SRP link has been created …"
 msgstr "SRP Link erstellt …"
 
-#: fleetpings/views.py:500
+#: fleetpings/views.py:452
 msgid "Form invalid. Please check your input."
 msgstr "Formular ungültig. Bitte die Angaben prüfen."
 
-#: fleetpings/views.py:502
+#: fleetpings/views.py:454
 msgid "No form data submitted."
 msgstr "Keine Formulardaten übermittelt."
```

### Comparing `aa_fleetpings-3.0.0/fleetpings/locale/es/LC_MESSAGES/django.mo` & `aa_fleetpings-3.0.0b1/fleetpings/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/locale/es/LC_MESSAGES/django.po` & `aa_fleetpings-3.0.0b1/fleetpings/locale/es/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,467 +4,467 @@
 # Zigor Fernandez Moreno <sietehierros@gmail.com>, 2023.
 # Peter Pfeufer <info@ppfeufer.de>, 2023.
 # Geovanny David Morales De la cruz <moralesgeovanny1996@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-15 21:21+0100\n"
+"POT-Creation-Date: 2023-10-01 17:17+0200\n"
 "PO-Revision-Date: 2023-10-25 07:04+0000\n"
-"Last-Translator: Geovanny David Morales De la cruz "
-"<moralesgeovanny1996@gmail.com>\n"
-"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-fleetpings/es/>\n"
+"Last-Translator: Geovanny David Morales De la cruz <moralesgeovanny1996@gmail"
+".com>\n"
+"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-fleetpings/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 5.1\n"
 
-#: fleetpings/__init__.py:10 fleetpings/templates/fleetpings/base.html:6
+#: fleetpings/__init__.py:12 fleetpings/templates/fleetpings/base.html:5
 #: fleetpings/templates/fleetpings/base.html:10
 msgid "Fleet Pings"
 msgstr "Pings de Flotas"
 
-#: fleetpings/admin.py:114 fleetpings/models.py:167
+#: fleetpings/admin.py:104 fleetpings/models.py:147
 msgid "Fleet comm"
 msgstr "Canal de comunicación de la flota"
 
-#: fleetpings/admin.py:144 fleetpings/form.py:151
+#: fleetpings/admin.py:125 fleetpings/form.py:149
 msgid "Doctrine"
 msgstr "Doctrina"
 
-#: fleetpings/admin.py:158 fleetpings/form.py:158 fleetpings/models.py:192
+#: fleetpings/admin.py:130 fleetpings/form.py:156 fleetpings/models.py:172
 msgid "Doctrine link"
 msgstr "Enlace de la Doctrina"
 
-#: fleetpings/admin.py:173 fleetpings/admin.py:244 fleetpings/admin.py:325
-#: fleetpings/admin.py:370 fleetpings/models.py:201 fleetpings/models.py:344
-#: fleetpings/models.py:451 fleetpings/models.py:522
+#: fleetpings/admin.py:136 fleetpings/admin.py:189 fleetpings/admin.py:243
+#: fleetpings/admin.py:288 fleetpings/models.py:181 fleetpings/models.py:308
+#: fleetpings/models.py:395 fleetpings/models.py:459
 msgid "Group restrictions"
 msgstr "Restricciones de grupo"
 
-#: fleetpings/admin.py:229 fleetpings/form.py:76
+#: fleetpings/admin.py:183 fleetpings/form.py:74
 #, fuzzy
 #| msgid "Ping Target"
 msgid "Ping target"
 msgstr "Destino del Ping"
 
-#: fleetpings/admin.py:289 fleetpings/form.py:93 fleetpings/models.py:485
+#: fleetpings/admin.py:225 fleetpings/form.py:91 fleetpings/models.py:422
 #, fuzzy
 #| msgid "Fleet Type"
 msgid "Fleet type"
 msgstr "Tipo de Flota"
 
-#: fleetpings/admin.py:303 fleetpings/models.py:442
+#: fleetpings/admin.py:230 fleetpings/models.py:386
 msgid "Embed color"
 msgstr "Color incrustado"
 
-#: fleetpings/admin.py:359 fleetpings/models.py:500
+#: fleetpings/admin.py:277 fleetpings/models.py:437
 msgid "Discord channel"
 msgstr "Canal de Discord"
 
-#: fleetpings/admin.py:364 fleetpings/models.py:513
+#: fleetpings/admin.py:282 fleetpings/models.py:450
 msgid "Webhook URL"
 msgstr "URL del webhook"
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: fleetpings/apps.py:21
 #, python-brace-format
 msgid "Fleet Pings v{__version__}"
 msgstr "Pings de Flota v{__version__}"
 
-#: fleetpings/form.py:27
+#: fleetpings/form.py:25
 msgid "Discord Markdown"
 msgstr "Markdown de Discord"
 
-#: fleetpings/form.py:34
+#: fleetpings/form.py:32
 #, python-brace-format
 msgid "Hint: You can use {discord_markdown_link} to format the text."
 msgstr "Pista: Puedes usar {discord_markdown_link} para dar formato al texto."
 
-#: fleetpings/form.py:78
+#: fleetpings/form.py:76
 msgid "Who do you want to ping?"
 msgstr "¿A quién quieres hacer ping?"
 
-#: fleetpings/form.py:83
+#: fleetpings/form.py:81
 msgid "Pre-Ping"
 msgstr "Pre-Ping"
 
-#: fleetpings/form.py:84
+#: fleetpings/form.py:82
 msgid "Mark this checkbox if this should be a pre-ping."
 msgstr "Marque esta casilla de verificación si esto es un pre-ping."
 
-#: fleetpings/form.py:88
+#: fleetpings/form.py:86
 #, fuzzy
 #| msgid "Ping To"
 msgid "Ping to"
 msgstr "Hacer Ping A"
 
-#: fleetpings/form.py:90
+#: fleetpings/form.py:88
 msgid "Select a channel to ping automatically."
 msgstr "Seleccione un canal para hacer ping automáticamente."
 
-#: fleetpings/form.py:97
+#: fleetpings/form.py:95
 msgid "FC name"
 msgstr ""
 
-#: fleetpings/form.py:99
+#: fleetpings/form.py:97
 msgid "Who is the FC?"
 msgstr "¿Quién es el FC?"
 
-#: fleetpings/form.py:103
+#: fleetpings/form.py:101
 #, fuzzy
 #| msgid "Fleet Name"
 msgid "Fleet name"
 msgstr "Nombre de la Flota"
 
-#: fleetpings/form.py:107
+#: fleetpings/form.py:105
 #, fuzzy
 #| msgid "What is the fleet name in fleet finder?"
 msgid "What is the fleet name in the fleet finder in Eve?"
 msgstr "¿Cuál es el nombre de la flota en el buscador de flotas?"
 
-#: fleetpings/form.py:113 fleetpings/models.py:305
+#: fleetpings/form.py:111 fleetpings/models.py:269
 #, fuzzy
 #| msgid "Formup Location"
 msgid "Formup location"
 msgstr "Ubicación para Formar"
 
-#: fleetpings/form.py:120
+#: fleetpings/form.py:118
 #, fuzzy
 #| msgid "Formup Time"
 msgid "Formup time"
 msgstr "Hora de Formar"
 
-#: fleetpings/form.py:124
+#: fleetpings/form.py:122
 msgid ""
 "To enable this field, either make it a pre-ping (checkbox above) or uncheck "
 "\"Formup NOW\" (checkbox below)."
 msgstr ""
 "Para habilitar este campo, conviértalo en Pre-Ping (casilla de verificación "
 "arriba) o desmarque «Formar AHORA» (casilla de verificación a continuación)."
 
-#: fleetpings/form.py:130
+#: fleetpings/form.py:128
 #, fuzzy
 #| msgid "Formup Timestamp"
 msgid "Formup timestamp"
 msgstr "Marca de Tiempo de Formar"
 
-#: fleetpings/form.py:136
+#: fleetpings/form.py:134
 msgid "Formup NOW"
 msgstr "Formar AHORA"
 
-#: fleetpings/form.py:138
+#: fleetpings/form.py:136
 msgid ""
 "If this checkbox is active, formup time will be set to \"NOW\" and the time "
 "in the field above (if any is set) will be ignored."
 msgstr ""
 "Si esta casilla de verificación está activa, el tiempo de formar se "
 "establecerá en «AHORA» y la hora en el campo de arriba (si se ha establecido "
 "alguna) será ignorada."
 
-#: fleetpings/form.py:144 fleetpings/models.py:168
+#: fleetpings/form.py:142 fleetpings/models.py:148
 #, fuzzy
 #| msgid "Fleet Comms"
 msgid "Fleet comms"
 msgstr "Canal de Comunicación de Flota"
 
-#: fleetpings/form.py:163
+#: fleetpings/form.py:161
 #, fuzzy
 #| msgid "Webhook Embed Color"
 msgid "Webhook embed color"
 msgstr "Color Incrustado del Webhook"
 
-#: fleetpings/form.py:169
+#: fleetpings/form.py:167
 msgid "SRP"
 msgstr "SRP"
 
-#: fleetpings/form.py:170
+#: fleetpings/form.py:168
 msgid "Is this fleet covered by SRP?"
 msgstr "¿Esta flota está cubierta por SRP?"
 
-#: fleetpings/form.py:175
+#: fleetpings/form.py:173
 #, fuzzy
 #| msgid "Create SRP Link"
 msgid "Create SRP link"
 msgstr "Crear el Enlace de SRP"
 
-#: fleetpings/form.py:177
+#: fleetpings/form.py:175
 msgid ""
 "If this checkbox is active, a SRP link specific for this fleet will be "
 "created.<br>Leave blank if unsure."
 msgstr ""
 "Si esta casilla de verificación está activa, se creará un enlace SRP "
 "específico para esta flota.<br>Deje en blanco si no está seguro."
 
-#: fleetpings/form.py:183
+#: fleetpings/form.py:181
 #, fuzzy
 #| msgid "Additional Information"
 msgid "Additional information"
 msgstr "Información Adicional"
 
-#: fleetpings/form.py:190
+#: fleetpings/form.py:188
 msgid "Feel free to add some more information about the fleet …"
 msgstr "Siéntase libre de agregar más información sobre la flota…"
 
-#: fleetpings/form.py:199
+#: fleetpings/form.py:197
 msgid "Create Optimer"
 msgstr "Crear Optiempo"
 
-#: fleetpings/form.py:201
+#: fleetpings/form.py:199
 msgid ""
 "If this checkbox is active, a fleet operations timer for this pre-ping will "
 "be created."
 msgstr ""
 "Si esta casilla de verificación está activa, se creará un temporizador de "
 "operaciones de flota para este pre-ping."
 
-#: fleetpings/models.py:41
+#: fleetpings/models.py:40
 msgid "You might want to install the Discord service first …"
 msgstr "Es posible que desee instalar primero el servicio de Discord …"
 
-#: fleetpings/models.py:49
+#: fleetpings/models.py:47
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr "¿Está seguro de que tiene su Discord vinculado a su Alliance Auth?"
 
-#: fleetpings/models.py:55
+#: fleetpings/models.py:51
 msgid "This group has not been synced to Discord yet."
 msgstr "Este grupo aún no se ha sincronizado con Discord."
 
-#: fleetpings/models.py:117
+#: fleetpings/models.py:104
 msgid "Can access this app"
 msgstr "Puede acceder esta aplicacion"
 
-#: fleetpings/models.py:127
+#: fleetpings/models.py:114
 msgid "Short name to identify this comms"
 msgstr "Nombre corto para identificar el canal de comunicación"
 
-#: fleetpings/models.py:128 fleetpings/models.py:184 fleetpings/models.py:272
-#: fleetpings/models.py:434
+#: fleetpings/models.py:115 fleetpings/models.py:164 fleetpings/models.py:242
+#: fleetpings/models.py:378
 msgid "Name"
 msgstr "Nombre"
 
-#: fleetpings/models.py:134
+#: fleetpings/models.py:121
 msgid "In which channel is the fleet?"
 msgstr "¿En qué canal está la flota?"
 
-#: fleetpings/models.py:135
+#: fleetpings/models.py:122
 msgid "Channel"
 msgstr "Canal"
 
-#: fleetpings/models.py:141 fleetpings/models.py:208 fleetpings/models.py:279
-#: fleetpings/models.py:351 fleetpings/models.py:458
+#: fleetpings/models.py:128 fleetpings/models.py:188 fleetpings/models.py:249
+#: fleetpings/models.py:315 fleetpings/models.py:402
 msgid "You can add notes about this configuration here if you want"
 msgstr "Puede agregar aquí notas sobre esta configuración si lo desea"
 
-#: fleetpings/models.py:142 fleetpings/models.py:209 fleetpings/models.py:280
-#: fleetpings/models.py:352 fleetpings/models.py:459 fleetpings/models.py:530
+#: fleetpings/models.py:129 fleetpings/models.py:189 fleetpings/models.py:250
+#: fleetpings/models.py:316 fleetpings/models.py:403 fleetpings/models.py:467
 msgid "Notes"
 msgstr "Notas"
 
-#: fleetpings/models.py:148
+#: fleetpings/models.py:135
 msgid "Whether this comms is enabled or not"
 msgstr "Si el canal de comunicaciones están habilitadas o no"
 
-#: fleetpings/models.py:149 fleetpings/models.py:217 fleetpings/models.py:288
-#: fleetpings/models.py:360 fleetpings/models.py:467 fleetpings/models.py:538
+#: fleetpings/models.py:136 fleetpings/models.py:197 fleetpings/models.py:258
+#: fleetpings/models.py:324 fleetpings/models.py:411 fleetpings/models.py:475
 msgid "Is enabled"
 msgstr "Está habilitado"
 
-#: fleetpings/models.py:183
+#: fleetpings/models.py:163
 msgid "Short name to identify this doctrine"
 msgstr "Nombre corto para identificar esta doctrina"
 
-#: fleetpings/models.py:191
+#: fleetpings/models.py:171
 msgid "A link to a doctrine page for this doctrine if you have."
 msgstr "El Enlace a la página de la doctrina, si tiene."
 
-#: fleetpings/models.py:200
+#: fleetpings/models.py:180
 msgid "Restrict this doctrine to the following groups …"
 msgstr "Restrinja esta doctrina a los siguientes grupos…"
 
-#: fleetpings/models.py:216
+#: fleetpings/models.py:196
 msgid "Whether this doctrine is enabled or not"
 msgstr "Si esta doctrina está habilitada o no"
 
-#: fleetpings/models.py:237
+#: fleetpings/models.py:214
 msgid "Your doctrine URL is not valid."
 msgstr "Su URL de doctrina no es válida."
 
-#: fleetpings/models.py:257
+#: fleetpings/models.py:227
 #, fuzzy
 #| msgid "Fleet Doctrine"
 msgid "Fleet doctrine"
 msgstr "Doctrina de Flota"
 
-#: fleetpings/models.py:258
+#: fleetpings/models.py:228
 #, fuzzy
 #| msgid "Fleet Doctrines"
 msgid "Fleet doctrines"
 msgstr "Doctrinas de Flota"
 
-#: fleetpings/models.py:271
+#: fleetpings/models.py:241
 msgid "Short name to identify this formup location"
 msgstr "Nombre corto para identificar la ubicación para formar"
 
-#: fleetpings/models.py:287 fleetpings/models.py:359
+#: fleetpings/models.py:257 fleetpings/models.py:323
 msgid "Whether this formup location is enabled or not"
 msgstr "Si esta ubicación para formar está habilitada o no"
 
-#: fleetpings/models.py:306
+#: fleetpings/models.py:270
 #, fuzzy
 #| msgid "Formup Locations"
 msgid "Formup locations"
 msgstr "Ubicaciones para Formar"
 
-#: fleetpings/models.py:322
+#: fleetpings/models.py:286
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 "Nombre del rol de Discord para hacer ping. (Nota: debe ser un grupo de "
 "autenticación sincronizado con Discord.)"
 
-#: fleetpings/models.py:326
+#: fleetpings/models.py:290
 msgid "Group name"
 msgstr "Nombre del grupo"
 
-#: fleetpings/models.py:334
+#: fleetpings/models.py:298
 msgid "ID of the Discord role to ping"
 msgstr "ID del rol de Discord para hacer ping"
 
-#: fleetpings/models.py:335
+#: fleetpings/models.py:299
 msgid "Discord ID"
 msgstr "ID de Discord"
 
-#: fleetpings/models.py:343 fleetpings/models.py:521
+#: fleetpings/models.py:307 fleetpings/models.py:458
 msgid "Restrict ping rights to the following groups …"
 msgstr "Restringir los derechos de ping a los siguientes grupos…"
 
-#: fleetpings/models.py:419
+#: fleetpings/models.py:363
 #, fuzzy
 #| msgid "Discord Ping Target"
 msgid "Discord ping target"
 msgstr "Destino del Ping de Discord"
 
-#: fleetpings/models.py:420
+#: fleetpings/models.py:364
 #, fuzzy
 #| msgid "Discord Ping Targets"
 msgid "Discord ping targets"
 msgstr "Destinos del Ping de Discord"
 
-#: fleetpings/models.py:433
+#: fleetpings/models.py:377
 msgid "Short name to identify this fleet type"
 msgstr "Nombre corto para identificar este tipo de flota"
 
-#: fleetpings/models.py:441
+#: fleetpings/models.py:385
 msgid "Highlight color for the embed"
 msgstr "Color resaltado para la incrustación"
 
-#: fleetpings/models.py:450
+#: fleetpings/models.py:394
 msgid "Restrict this fleet type to the following groups …"
 msgstr "Restrinja este tipo de flota a los siguientes grupos…"
 
-#: fleetpings/models.py:466
+#: fleetpings/models.py:410
 msgid "Whether this fleet type is enabled or not"
 msgstr "Si este tipo de flota está habilitado o no"
 
-#: fleetpings/models.py:486
+#: fleetpings/models.py:423
 #, fuzzy
 #| msgid "Fleet Types"
 msgid "Fleet types"
 msgstr "Tipos de Flota"
 
-#: fleetpings/models.py:499
+#: fleetpings/models.py:436
 msgid "Name of the channel this webhook posts to"
 msgstr "Nombre del canal en el que publica este webhook"
 
-#: fleetpings/models.py:509
+#: fleetpings/models.py:446
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
 "URL de este webhook, p.ej. https://discord.com/api/webhooks/123456/abcdef"
 
-#: fleetpings/models.py:529
+#: fleetpings/models.py:466
 msgid "You can add notes about this webhook here if you want"
 msgstr "Puede agregar aquí notas sobre este webhook si lo desea"
 
-#: fleetpings/models.py:537
+#: fleetpings/models.py:474
 msgid "Whether this webhook is active or not"
 msgstr "Si este webhook está activo o no"
 
-#: fleetpings/models.py:556
+#: fleetpings/models.py:486
 msgid "Webhook"
 msgstr "Webhook"
 
-#: fleetpings/models.py:557
+#: fleetpings/models.py:487
 msgid "Webhooks"
 msgstr "Webhooks"
 
-#: fleetpings/models.py:576
+#: fleetpings/models.py:502
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 "URL de webhook no válida. La URL del webhook que ingresó no coincide con "
 "ningún formato conocido para un webhook de Discord. Compruebe la URL del "
 "webhook."
 
-#: fleetpings/models.py:596
+#: fleetpings/models.py:522
 msgid "Use default fleet types"
 msgstr "Usar tipos de flota predeterminados"
 
-#: fleetpings/models.py:599
+#: fleetpings/models.py:525
 msgid "Use default ping targets"
 msgstr "Usar objetivos de ping predeterminados"
 
-#: fleetpings/models.py:602
+#: fleetpings/models.py:528
 msgid "Use Doctrines from Fittings module"
 msgstr "Usar doctrinas del módulo Fiteos"
 
-#: fleetpings/models.py:604
+#: fleetpings/models.py:530
 #, fuzzy
 #| msgid "Verify Webhooks"
 msgid "Verify webhooks"
 msgstr "Verificar Webhooks"
 
-#: fleetpings/models.py:605
+#: fleetpings/models.py:531
 msgid "Default embed color"
 msgstr "Color incrustado predeterminado"
 
-#: fleetpings/models.py:611
+#: fleetpings/models.py:537
 msgid ""
 "Whether to use default fleet types. If checked, the default fleet types "
 "(Roaming, Home Defense, StratOP, and CTA) will be added to the Fleet Type "
 "dropdown."
 msgstr ""
 "Ya sea para usar tipos de flota predeterminados. Si está marcado, los tipos "
 "de flota predeterminados (Roaming, Home Defense, StratOP y CTA) se agregarán "
 "al menú desplegable Tipo de flota."
 
-#: fleetpings/models.py:622
+#: fleetpings/models.py:548
 msgid ""
 "Whether to use default ping targets. If checked, the default ping targets "
 "(@everyone and @here) will be added to the Ping Target dropdown."
 msgstr ""
 "a sea para usar objetivos de ping predeterminados. Si está marcado, los "
 "destinos de ping predeterminados (@everyone and @here) se agregarán al menú "
 "desplegable Destino de ping."
 
-#: fleetpings/models.py:632
+#: fleetpings/models.py:558
 msgid ""
 "Whether to use the doctrines from the Fittings modules in the doctrine "
 "dropdown. Note: The fittings module needs to be installed for this."
 msgstr ""
 "Si usar las doctrinas de los módulos de Fiteos en el menú desplegable de "
 "doctrinas. Nota: Para ello, es necesario instalar el módulo de fiteos."
 
-#: fleetpings/models.py:642
+#: fleetpings/models.py:568
 #, fuzzy
 #| msgid ""
 #| "Whether to verify Webhooks URLs or not. Note: When unchecked Webhook URLs "
 #| "will not be verified, so the app can be used with non-Discord Webhooks as "
 #| "well. When disabling webhook verification and using non-Discord webhooks, "
 #| "it is up to you to make sure your webhook understands a payload that is "
 #| "formatted for Discord webhooks."
@@ -478,83 +478,83 @@
 "Si verificar o no las URL de Webhooks. Nota: Cuando las URL de Webhook no "
 "estén marcadas, no se verificarán, por lo que la aplicación también se puede "
 "usar con Webhooks que no sean de Discord. Al deshabilitar la verificación de "
 "webhooks y usar webhooks que no sean de Discord, depende de usted asegurarse "
 "de que su webhook comprenda una carga útil con formato para webhooks de "
 "Discord."
 
-#: fleetpings/models.py:655
+#: fleetpings/models.py:581
 msgid "Default highlight color for the webhook embed."
 msgstr "Color resaltado predeterminado para la inserción de webhook."
 
-#: fleetpings/models.py:667
+#: fleetpings/models.py:593
 #, fuzzy
 #| msgid "setting"
 msgid "Setting"
 msgstr "ajuste"
 
-#: fleetpings/models.py:668
+#: fleetpings/models.py:594
 #, fuzzy
 #| msgid "settings"
 msgid "Settings"
 msgstr "ajustes"
 
-#: fleetpings/models.py:678
+#: fleetpings/models.py:597
 msgid "Fleet Pings Settings"
 msgstr "Ajustes de Pings de Flota"
 
 #: fleetpings/templates/fleetpings/index.html:11
 #, fuzzy
 #| msgid "Fleet Information"
 msgid "Fleet information"
 msgstr "Información de Flota"
 
-#: fleetpings/templates/fleetpings/index.html:23
+#: fleetpings/templates/fleetpings/index.html:22
 #, fuzzy
 #| msgid "Formatted Ping Text"
 msgid "Formatted ping text"
 msgstr "Formato de Texto para el Ping"
 
-#: fleetpings/templates/fleetpings/index.html:51
+#: fleetpings/templates/fleetpings/index.html:49
 #, fuzzy
 #| msgid ""
 #| "Mandatory information is missing. To create an optimer, you need to "
 #| "provide all of the following information:<br>» FC Name<br>» Fleet "
 #| "Name<br>» Formup Location<br>» Formup Time<br>» Ships / Doctrine"
 msgid ""
 "Mandatory information is missing. To create an optimer, you need to provide "
 "all of the following information:<br>» FC name<br>» Fleet name<br>» Formup "
 "location<br>» Formup time<br>» Ships / Doctrine"
 msgstr ""
 "Falta información obligatoria. Para crear un optiempo, debe proporcionar "
 "toda la siguiente información:<br>» Nombre del FC<br>» Nombre de la "
 "flota<br>» Ubicación para formar<br>» Hora para formar<br>» Naves / Doctrina"
 
-#: fleetpings/templates/fleetpings/index.html:56
+#: fleetpings/templates/fleetpings/index.html:54
 #, fuzzy
 #| msgid ""
 #| "Mandatory information is missing. To create an SRP link, you need to "
 #| "provide all of the following information:<br>» Fleet Name<br>» Ships / "
 #| "Doctrine"
 msgid ""
 "Mandatory information is missing. To create an SRP link, you need to provide "
 "all of the following information:<br>» Fleet name<br>» Ships / Doctrine"
 msgstr ""
 "Falta información obligatoria. Para crear un enlace SRP, debe proporcionar "
 "toda la siguiente información:<br>» Nombre de la flota<br>» Naves / Doctrina"
 
-#: fleetpings/templates/fleetpings/index.html:60
+#: fleetpings/templates/fleetpings/index.html:58
 msgid ""
 "Error! Your ping was not copied to your clipboard. Maybe your browser "
 "doesn&apos;t support this feature."
 msgstr ""
 "Error! Su ping no se copió en su portapapeles. Tal vez su navegador no "
 "admita esta función."
 
-#: fleetpings/templates/fleetpings/index.html:61
+#: fleetpings/templates/fleetpings/index.html:59
 msgid ""
 "Success! Your ping text has been copied to your clipboard. Now be a good FC "
 "and throw it in your chat so you actually get some people in fleet."
 msgstr ""
 "Éxito! Su texto de ping ha sido copiado a su portapapeles. Ahora sea un buen "
 "FC y póngalo en su chat para que realmente tenga algunas personas en la "
 "flota."
@@ -567,69 +567,57 @@
 "¿Quieres ayudar a traducir esta aplicación a tu idioma o mejorar la "
 "traducción existente?"
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "¡Únete a nuestro equipo de traductores!"
 
-#: fleetpings/templates/fleetpings/partials/form/form.html:69
+#: fleetpings/templates/fleetpings/partials/form/form.html:68
 #, fuzzy
 #| msgid "Create Ping"
 msgid "Create ping"
 msgstr "Crear Ping"
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:6
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:7
 msgid "Please think twice if you really need to ping <code>@everyone</code>."
 msgstr ""
 "Piénselo dos veces si realmente necesita hacer ping <code>@everyone</code>."
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:10
-#, fuzzy
-#| msgid ""
-#| "\n"
-#| "                    <code>@everyone</code>\n"
-#| "                    includes also all the people in this channel who are "
-#| "offline and\n"
-#| "                    possibly asleep at the moment and might be waking up "
-#| "when their\n"
-#| "                    mobile devices ping. Or they wake up hours later to "
-#| "irrelevant\n"
-#| "                    pings by the time they open Discord.\n"
-#| "                "
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:11
 msgid ""
 "\n"
-"                <code>@everyone</code>\n"
-"                includes also all the people in this channel who are offline "
-"and\n"
-"                possibly asleep at the moment and might be waking up when "
-"their\n"
-"                mobile devices ping. Or they wake up hours later to "
+"                    <code>@everyone</code>\n"
+"                    includes also all the people in this channel who are "
+"offline and\n"
+"                    possibly asleep at the moment and might be waking up "
+"when their\n"
+"                    mobile devices ping. Or they wake up hours later to "
 "irrelevant\n"
-"                pings by the time they open Discord.\n"
-"            "
+"                    pings by the time they open Discord.\n"
+"                "
 msgstr ""
 "\n"
 "                    <code>@everyone</code>\n"
 "                    incluye también a todas las personas en este canal que "
 "están fuera de línea y\n"
 "                    posiblemente dormidas en este momento y podrían estar "
 "despertando mediante sus\n"
 "                    dispositivos móviles para pings. O se despiertan horas "
 "más tarde con cosas irrelevantes\n"
 "                    con los pings en el momento en que abren Discord.\n"
 "                "
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:20
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:21
 msgid ""
 "Notification spam is a real thing and might entice people to mute channels."
 msgstr ""
 "El spam es algo real en las notificaciones y puede hacer que las personas "
 "silencien los canales."
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:24
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:25
 msgid "<code>@here</code> usually does the trick just fine."
 msgstr "<code>@here</code> engaña muy bien por lo general."
 
 #: fleetpings/templates/fleetpings/partials/form/segments/fleet-type.html:3
 msgid "Please select"
 msgstr "Por favor selecciona"
 
@@ -673,27 +661,27 @@
 
 #: fleetpings/templates/fleetpings/partials/ping/ping.html:22
 #, fuzzy
 #| msgid "Copy Ping Text"
 msgid "Copy ping text"
 msgstr "Copiar el Texto de Ping"
 
-#: fleetpings/views.py:439
+#: fleetpings/views.py:394
 msgid "Not all mandatory information available to create an SRP link."
 msgstr ""
 "No toda la información obligatoria está disponible para crear un enlace SRP."
 
-#: fleetpings/views.py:474
+#: fleetpings/views.py:426
 msgid "Fleet operations timer has been created …"
 msgstr "Se ha creado el temporizador de operaciones de flota…"
 
-#: fleetpings/views.py:483
+#: fleetpings/views.py:435
 msgid "SRP link has been created …"
 msgstr "Se ha creado el enlace SRP…"
 
-#: fleetpings/views.py:500
+#: fleetpings/views.py:452
 msgid "Form invalid. Please check your input."
 msgstr "Formulario inválido. Por favor, compruebe su entrada."
 
-#: fleetpings/views.py:502
+#: fleetpings/views.py:454
 msgid "No form data submitted."
 msgstr "No se enviaron datos del formulario."
```

### Comparing `aa_fleetpings-3.0.0/fleetpings/locale/fr_FR/LC_MESSAGES/django.mo` & `aa_fleetpings-3.0.0b1/fleetpings/locale/fr_FR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/locale/fr_FR/LC_MESSAGES/django.po` & `aa_fleetpings-3.0.0b1/fleetpings/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,457 +3,457 @@
 # This file is distributed under the same license as the PACKAGE package.
 # erka Ekanon <M6musicT@hotmail.fr>, 2024.
 # Peter Pfeufer <info@ppfeufer.de>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-15 21:21+0100\n"
+"POT-Creation-Date: 2023-10-01 17:17+0200\n"
 "PO-Revision-Date: 2024-01-12 19:05+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: French <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-fleetpings/fr/>\n"
+"Language-Team: French <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-fleetpings/fr/>\n"
 "Language: fr_FR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
 "X-Generator: Weblate 5.3.1\n"
 
-#: fleetpings/__init__.py:10 fleetpings/templates/fleetpings/base.html:6
+#: fleetpings/__init__.py:12 fleetpings/templates/fleetpings/base.html:5
 #: fleetpings/templates/fleetpings/base.html:10
 msgid "Fleet Pings"
 msgstr ""
 
-#: fleetpings/admin.py:114 fleetpings/models.py:167
+#: fleetpings/admin.py:104 fleetpings/models.py:147
 msgid "Fleet comm"
 msgstr ""
 
-#: fleetpings/admin.py:144 fleetpings/form.py:151
+#: fleetpings/admin.py:125 fleetpings/form.py:149
 msgid "Doctrine"
 msgstr ""
 
-#: fleetpings/admin.py:158 fleetpings/form.py:158 fleetpings/models.py:192
+#: fleetpings/admin.py:130 fleetpings/form.py:156 fleetpings/models.py:172
 msgid "Doctrine link"
 msgstr ""
 
-#: fleetpings/admin.py:173 fleetpings/admin.py:244 fleetpings/admin.py:325
-#: fleetpings/admin.py:370 fleetpings/models.py:201 fleetpings/models.py:344
-#: fleetpings/models.py:451 fleetpings/models.py:522
+#: fleetpings/admin.py:136 fleetpings/admin.py:189 fleetpings/admin.py:243
+#: fleetpings/admin.py:288 fleetpings/models.py:181 fleetpings/models.py:308
+#: fleetpings/models.py:395 fleetpings/models.py:459
 msgid "Group restrictions"
 msgstr ""
 
-#: fleetpings/admin.py:229 fleetpings/form.py:76
+#: fleetpings/admin.py:183 fleetpings/form.py:74
 msgid "Ping target"
 msgstr ""
 
-#: fleetpings/admin.py:289 fleetpings/form.py:93 fleetpings/models.py:485
+#: fleetpings/admin.py:225 fleetpings/form.py:91 fleetpings/models.py:422
 msgid "Fleet type"
 msgstr ""
 
-#: fleetpings/admin.py:303 fleetpings/models.py:442
+#: fleetpings/admin.py:230 fleetpings/models.py:386
 msgid "Embed color"
 msgstr ""
 
-#: fleetpings/admin.py:359 fleetpings/models.py:500
+#: fleetpings/admin.py:277 fleetpings/models.py:437
 msgid "Discord channel"
 msgstr ""
 
-#: fleetpings/admin.py:364 fleetpings/models.py:513
+#: fleetpings/admin.py:282 fleetpings/models.py:450
 msgid "Webhook URL"
 msgstr ""
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: fleetpings/apps.py:21
 #, python-brace-format
 msgid "Fleet Pings v{__version__}"
 msgstr ""
 
-#: fleetpings/form.py:27
+#: fleetpings/form.py:25
 msgid "Discord Markdown"
 msgstr ""
 
-#: fleetpings/form.py:34
+#: fleetpings/form.py:32
 #, python-brace-format
 msgid "Hint: You can use {discord_markdown_link} to format the text."
 msgstr ""
 
-#: fleetpings/form.py:78
+#: fleetpings/form.py:76
 msgid "Who do you want to ping?"
 msgstr ""
 
-#: fleetpings/form.py:83
+#: fleetpings/form.py:81
 msgid "Pre-Ping"
 msgstr ""
 
-#: fleetpings/form.py:84
+#: fleetpings/form.py:82
 msgid "Mark this checkbox if this should be a pre-ping."
 msgstr ""
 
-#: fleetpings/form.py:88
+#: fleetpings/form.py:86
 msgid "Ping to"
 msgstr ""
 
-#: fleetpings/form.py:90
+#: fleetpings/form.py:88
 msgid "Select a channel to ping automatically."
 msgstr ""
 
-#: fleetpings/form.py:97
+#: fleetpings/form.py:95
 msgid "FC name"
 msgstr ""
 
-#: fleetpings/form.py:99
+#: fleetpings/form.py:97
 msgid "Who is the FC?"
 msgstr ""
 
-#: fleetpings/form.py:103
+#: fleetpings/form.py:101
 msgid "Fleet name"
 msgstr ""
 
-#: fleetpings/form.py:107
+#: fleetpings/form.py:105
 msgid "What is the fleet name in the fleet finder in Eve?"
 msgstr ""
 
-#: fleetpings/form.py:113 fleetpings/models.py:305
+#: fleetpings/form.py:111 fleetpings/models.py:269
 msgid "Formup location"
 msgstr ""
 
-#: fleetpings/form.py:120
+#: fleetpings/form.py:118
 msgid "Formup time"
 msgstr ""
 
-#: fleetpings/form.py:124
+#: fleetpings/form.py:122
 msgid ""
 "To enable this field, either make it a pre-ping (checkbox above) or uncheck "
 "\"Formup NOW\" (checkbox below)."
 msgstr ""
 
-#: fleetpings/form.py:130
+#: fleetpings/form.py:128
 msgid "Formup timestamp"
 msgstr ""
 
-#: fleetpings/form.py:136
+#: fleetpings/form.py:134
 msgid "Formup NOW"
 msgstr ""
 
-#: fleetpings/form.py:138
+#: fleetpings/form.py:136
 msgid ""
 "If this checkbox is active, formup time will be set to \"NOW\" and the time "
 "in the field above (if any is set) will be ignored."
 msgstr ""
 
-#: fleetpings/form.py:144 fleetpings/models.py:168
+#: fleetpings/form.py:142 fleetpings/models.py:148
 msgid "Fleet comms"
 msgstr ""
 
-#: fleetpings/form.py:163
+#: fleetpings/form.py:161
 msgid "Webhook embed color"
 msgstr ""
 
-#: fleetpings/form.py:169
+#: fleetpings/form.py:167
 msgid "SRP"
 msgstr ""
 
-#: fleetpings/form.py:170
+#: fleetpings/form.py:168
 msgid "Is this fleet covered by SRP?"
 msgstr ""
 
-#: fleetpings/form.py:175
+#: fleetpings/form.py:173
 msgid "Create SRP link"
 msgstr ""
 
-#: fleetpings/form.py:177
+#: fleetpings/form.py:175
 msgid ""
 "If this checkbox is active, a SRP link specific for this fleet will be "
 "created.<br>Leave blank if unsure."
 msgstr ""
 
-#: fleetpings/form.py:183
+#: fleetpings/form.py:181
 msgid "Additional information"
 msgstr ""
 
-#: fleetpings/form.py:190
+#: fleetpings/form.py:188
 msgid "Feel free to add some more information about the fleet …"
 msgstr ""
 
-#: fleetpings/form.py:199
+#: fleetpings/form.py:197
 msgid "Create Optimer"
 msgstr ""
 
-#: fleetpings/form.py:201
+#: fleetpings/form.py:199
 msgid ""
 "If this checkbox is active, a fleet operations timer for this pre-ping will "
 "be created."
 msgstr ""
 
-#: fleetpings/models.py:41
+#: fleetpings/models.py:40
 msgid "You might want to install the Discord service first …"
 msgstr ""
 
-#: fleetpings/models.py:49
+#: fleetpings/models.py:47
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
 
-#: fleetpings/models.py:55
+#: fleetpings/models.py:51
 msgid "This group has not been synced to Discord yet."
 msgstr ""
 
-#: fleetpings/models.py:117
+#: fleetpings/models.py:104
 msgid "Can access this app"
 msgstr "Peut accéder à cette application"
 
-#: fleetpings/models.py:127
+#: fleetpings/models.py:114
 msgid "Short name to identify this comms"
 msgstr ""
 
-#: fleetpings/models.py:128 fleetpings/models.py:184 fleetpings/models.py:272
-#: fleetpings/models.py:434
+#: fleetpings/models.py:115 fleetpings/models.py:164 fleetpings/models.py:242
+#: fleetpings/models.py:378
 msgid "Name"
 msgstr ""
 
-#: fleetpings/models.py:134
+#: fleetpings/models.py:121
 msgid "In which channel is the fleet?"
 msgstr ""
 
-#: fleetpings/models.py:135
+#: fleetpings/models.py:122
 msgid "Channel"
 msgstr ""
 
-#: fleetpings/models.py:141 fleetpings/models.py:208 fleetpings/models.py:279
-#: fleetpings/models.py:351 fleetpings/models.py:458
+#: fleetpings/models.py:128 fleetpings/models.py:188 fleetpings/models.py:249
+#: fleetpings/models.py:315 fleetpings/models.py:402
 msgid "You can add notes about this configuration here if you want"
 msgstr ""
 
-#: fleetpings/models.py:142 fleetpings/models.py:209 fleetpings/models.py:280
-#: fleetpings/models.py:352 fleetpings/models.py:459 fleetpings/models.py:530
+#: fleetpings/models.py:129 fleetpings/models.py:189 fleetpings/models.py:250
+#: fleetpings/models.py:316 fleetpings/models.py:403 fleetpings/models.py:467
 msgid "Notes"
 msgstr ""
 
-#: fleetpings/models.py:148
+#: fleetpings/models.py:135
 msgid "Whether this comms is enabled or not"
 msgstr ""
 
-#: fleetpings/models.py:149 fleetpings/models.py:217 fleetpings/models.py:288
-#: fleetpings/models.py:360 fleetpings/models.py:467 fleetpings/models.py:538
+#: fleetpings/models.py:136 fleetpings/models.py:197 fleetpings/models.py:258
+#: fleetpings/models.py:324 fleetpings/models.py:411 fleetpings/models.py:475
 msgid "Is enabled"
 msgstr ""
 
-#: fleetpings/models.py:183
+#: fleetpings/models.py:163
 msgid "Short name to identify this doctrine"
 msgstr ""
 
-#: fleetpings/models.py:191
+#: fleetpings/models.py:171
 msgid "A link to a doctrine page for this doctrine if you have."
 msgstr ""
 
-#: fleetpings/models.py:200
+#: fleetpings/models.py:180
 msgid "Restrict this doctrine to the following groups …"
 msgstr ""
 
-#: fleetpings/models.py:216
+#: fleetpings/models.py:196
 msgid "Whether this doctrine is enabled or not"
 msgstr ""
 
-#: fleetpings/models.py:237
+#: fleetpings/models.py:214
 msgid "Your doctrine URL is not valid."
 msgstr ""
 
-#: fleetpings/models.py:257
+#: fleetpings/models.py:227
 msgid "Fleet doctrine"
 msgstr ""
 
-#: fleetpings/models.py:258
+#: fleetpings/models.py:228
 msgid "Fleet doctrines"
 msgstr ""
 
-#: fleetpings/models.py:271
+#: fleetpings/models.py:241
 msgid "Short name to identify this formup location"
 msgstr ""
 
-#: fleetpings/models.py:287 fleetpings/models.py:359
+#: fleetpings/models.py:257 fleetpings/models.py:323
 msgid "Whether this formup location is enabled or not"
 msgstr ""
 
-#: fleetpings/models.py:306
+#: fleetpings/models.py:270
 msgid "Formup locations"
 msgstr ""
 
-#: fleetpings/models.py:322
+#: fleetpings/models.py:286
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 
-#: fleetpings/models.py:326
+#: fleetpings/models.py:290
 msgid "Group name"
 msgstr ""
 
-#: fleetpings/models.py:334
+#: fleetpings/models.py:298
 msgid "ID of the Discord role to ping"
 msgstr ""
 
-#: fleetpings/models.py:335
+#: fleetpings/models.py:299
 msgid "Discord ID"
 msgstr ""
 
-#: fleetpings/models.py:343 fleetpings/models.py:521
+#: fleetpings/models.py:307 fleetpings/models.py:458
 msgid "Restrict ping rights to the following groups …"
 msgstr ""
 
-#: fleetpings/models.py:419
+#: fleetpings/models.py:363
 msgid "Discord ping target"
 msgstr ""
 
-#: fleetpings/models.py:420
+#: fleetpings/models.py:364
 msgid "Discord ping targets"
 msgstr ""
 
-#: fleetpings/models.py:433
+#: fleetpings/models.py:377
 msgid "Short name to identify this fleet type"
 msgstr ""
 
-#: fleetpings/models.py:441
+#: fleetpings/models.py:385
 msgid "Highlight color for the embed"
 msgstr ""
 
-#: fleetpings/models.py:450
+#: fleetpings/models.py:394
 msgid "Restrict this fleet type to the following groups …"
 msgstr ""
 
-#: fleetpings/models.py:466
+#: fleetpings/models.py:410
 msgid "Whether this fleet type is enabled or not"
 msgstr ""
 
-#: fleetpings/models.py:486
+#: fleetpings/models.py:423
 msgid "Fleet types"
 msgstr ""
 
-#: fleetpings/models.py:499
+#: fleetpings/models.py:436
 msgid "Name of the channel this webhook posts to"
 msgstr ""
 
-#: fleetpings/models.py:509
+#: fleetpings/models.py:446
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
 
-#: fleetpings/models.py:529
+#: fleetpings/models.py:466
 msgid "You can add notes about this webhook here if you want"
 msgstr ""
 
-#: fleetpings/models.py:537
+#: fleetpings/models.py:474
 msgid "Whether this webhook is active or not"
 msgstr ""
 
-#: fleetpings/models.py:556
+#: fleetpings/models.py:486
 msgid "Webhook"
 msgstr ""
 
-#: fleetpings/models.py:557
+#: fleetpings/models.py:487
 msgid "Webhooks"
 msgstr ""
 
-#: fleetpings/models.py:576
+#: fleetpings/models.py:502
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 
-#: fleetpings/models.py:596
+#: fleetpings/models.py:522
 msgid "Use default fleet types"
 msgstr ""
 
-#: fleetpings/models.py:599
+#: fleetpings/models.py:525
 msgid "Use default ping targets"
 msgstr ""
 
-#: fleetpings/models.py:602
+#: fleetpings/models.py:528
 msgid "Use Doctrines from Fittings module"
 msgstr ""
 
-#: fleetpings/models.py:604
+#: fleetpings/models.py:530
 msgid "Verify webhooks"
 msgstr ""
 
-#: fleetpings/models.py:605
+#: fleetpings/models.py:531
 msgid "Default embed color"
 msgstr ""
 
-#: fleetpings/models.py:611
+#: fleetpings/models.py:537
 msgid ""
 "Whether to use default fleet types. If checked, the default fleet types "
 "(Roaming, Home Defense, StratOP, and CTA) will be added to the Fleet Type "
 "dropdown."
 msgstr ""
 
-#: fleetpings/models.py:622
+#: fleetpings/models.py:548
 msgid ""
 "Whether to use default ping targets. If checked, the default ping targets "
 "(@everyone and @here) will be added to the Ping Target dropdown."
 msgstr ""
 
-#: fleetpings/models.py:632
+#: fleetpings/models.py:558
 msgid ""
 "Whether to use the doctrines from the Fittings modules in the doctrine "
 "dropdown. Note: The fittings module needs to be installed for this."
 msgstr ""
 
-#: fleetpings/models.py:642
+#: fleetpings/models.py:568
 msgid ""
 "Whether to verify webhooks URLs or not. Note: When unchecked, webhook URLs "
 "will not be verified, so the app can be used with non-Discord webhooks as "
 "well. When disabling webhook verification and using non-Discord webhooks, it "
 "is up to you to make sure your webhook understands a payload that is "
 "formatted for Discord webhooks."
 msgstr ""
 
-#: fleetpings/models.py:655
+#: fleetpings/models.py:581
 msgid "Default highlight color for the webhook embed."
 msgstr ""
 
-#: fleetpings/models.py:667
+#: fleetpings/models.py:593
 msgid "Setting"
 msgstr ""
 
-#: fleetpings/models.py:668
+#: fleetpings/models.py:594
 msgid "Settings"
 msgstr ""
 
-#: fleetpings/models.py:678
+#: fleetpings/models.py:597
 msgid "Fleet Pings Settings"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/index.html:11
 msgid "Fleet information"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/index.html:23
+#: fleetpings/templates/fleetpings/index.html:22
 msgid "Formatted ping text"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/index.html:51
+#: fleetpings/templates/fleetpings/index.html:49
 msgid ""
 "Mandatory information is missing. To create an optimer, you need to provide "
 "all of the following information:<br>» FC name<br>» Fleet name<br>» Formup "
 "location<br>» Formup time<br>» Ships / Doctrine"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/index.html:56
+#: fleetpings/templates/fleetpings/index.html:54
 msgid ""
 "Mandatory information is missing. To create an SRP link, you need to provide "
 "all of the following information:<br>» Fleet name<br>» Ships / Doctrine"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/index.html:60
+#: fleetpings/templates/fleetpings/index.html:58
 msgid ""
 "Error! Your ping was not copied to your clipboard. Maybe your browser "
 "doesn&apos;t support this feature."
 msgstr ""
 
-#: fleetpings/templates/fleetpings/index.html:61
+#: fleetpings/templates/fleetpings/index.html:59
 msgid ""
 "Success! Your ping text has been copied to your clipboard. Now be a good FC "
 "and throw it in your chat so you actually get some people in fleet."
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:5
 msgid ""
@@ -463,42 +463,42 @@
 "Voulez-vous aider à traduire cette application dans votre langue ou "
 "améliorer la traduction existante ?"
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "Rejoignez notre équipe de traducteurs !"
 
-#: fleetpings/templates/fleetpings/partials/form/form.html:69
+#: fleetpings/templates/fleetpings/partials/form/form.html:68
 msgid "Create ping"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:6
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:7
 msgid "Please think twice if you really need to ping <code>@everyone</code>."
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:10
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:11
 msgid ""
 "\n"
-"                <code>@everyone</code>\n"
-"                includes also all the people in this channel who are offline "
-"and\n"
-"                possibly asleep at the moment and might be waking up when "
-"their\n"
-"                mobile devices ping. Or they wake up hours later to "
+"                    <code>@everyone</code>\n"
+"                    includes also all the people in this channel who are "
+"offline and\n"
+"                    possibly asleep at the moment and might be waking up "
+"when their\n"
+"                    mobile devices ping. Or they wake up hours later to "
 "irrelevant\n"
-"                pings by the time they open Discord.\n"
-"            "
+"                    pings by the time they open Discord.\n"
+"                "
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:20
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:21
 msgid ""
 "Notification spam is a real thing and might entice people to mute channels."
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:24
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:25
 msgid "<code>@here</code> usually does the trick just fine."
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/form/segments/fleet-type.html:3
 msgid "Please select"
 msgstr ""
 
@@ -538,26 +538,26 @@
 msgid "No ping created yet …"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/ping/ping.html:22
 msgid "Copy ping text"
 msgstr ""
 
-#: fleetpings/views.py:439
+#: fleetpings/views.py:394
 msgid "Not all mandatory information available to create an SRP link."
 msgstr ""
 
-#: fleetpings/views.py:474
+#: fleetpings/views.py:426
 msgid "Fleet operations timer has been created …"
 msgstr ""
 
-#: fleetpings/views.py:483
+#: fleetpings/views.py:435
 msgid "SRP link has been created …"
 msgstr ""
 
-#: fleetpings/views.py:500
+#: fleetpings/views.py:452
 msgid "Form invalid. Please check your input."
 msgstr ""
 
-#: fleetpings/views.py:502
+#: fleetpings/views.py:454
 msgid "No form data submitted."
 msgstr ""
```

### Comparing `aa_fleetpings-3.0.0/fleetpings/locale/it_IT/LC_MESSAGES/django.po` & `aa_fleetpings-3.0.0b1/fleetpings/locale/ja/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -3,457 +3,457 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-15 21:21+0100\n"
+"POT-Creation-Date: 2023-10-01 17:17+0200\n"
 "PO-Revision-Date: 2023-09-24 13:14+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-fleetpings/it/>\n"
-"Language: it_IT\n"
+"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-fleetpings/ja/>\n"
+"Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "X-Generator: Weblate 5.0.2\n"
 
-#: fleetpings/__init__.py:10 fleetpings/templates/fleetpings/base.html:6
+#: fleetpings/__init__.py:12 fleetpings/templates/fleetpings/base.html:5
 #: fleetpings/templates/fleetpings/base.html:10
 msgid "Fleet Pings"
 msgstr ""
 
-#: fleetpings/admin.py:114 fleetpings/models.py:167
+#: fleetpings/admin.py:104 fleetpings/models.py:147
 msgid "Fleet comm"
 msgstr ""
 
-#: fleetpings/admin.py:144 fleetpings/form.py:151
+#: fleetpings/admin.py:125 fleetpings/form.py:149
 msgid "Doctrine"
 msgstr ""
 
-#: fleetpings/admin.py:158 fleetpings/form.py:158 fleetpings/models.py:192
+#: fleetpings/admin.py:130 fleetpings/form.py:156 fleetpings/models.py:172
 msgid "Doctrine link"
 msgstr ""
 
-#: fleetpings/admin.py:173 fleetpings/admin.py:244 fleetpings/admin.py:325
-#: fleetpings/admin.py:370 fleetpings/models.py:201 fleetpings/models.py:344
-#: fleetpings/models.py:451 fleetpings/models.py:522
+#: fleetpings/admin.py:136 fleetpings/admin.py:189 fleetpings/admin.py:243
+#: fleetpings/admin.py:288 fleetpings/models.py:181 fleetpings/models.py:308
+#: fleetpings/models.py:395 fleetpings/models.py:459
 msgid "Group restrictions"
 msgstr ""
 
-#: fleetpings/admin.py:229 fleetpings/form.py:76
+#: fleetpings/admin.py:183 fleetpings/form.py:74
 msgid "Ping target"
 msgstr ""
 
-#: fleetpings/admin.py:289 fleetpings/form.py:93 fleetpings/models.py:485
+#: fleetpings/admin.py:225 fleetpings/form.py:91 fleetpings/models.py:422
 msgid "Fleet type"
 msgstr ""
 
-#: fleetpings/admin.py:303 fleetpings/models.py:442
+#: fleetpings/admin.py:230 fleetpings/models.py:386
 msgid "Embed color"
 msgstr ""
 
-#: fleetpings/admin.py:359 fleetpings/models.py:500
+#: fleetpings/admin.py:277 fleetpings/models.py:437
 msgid "Discord channel"
 msgstr ""
 
-#: fleetpings/admin.py:364 fleetpings/models.py:513
+#: fleetpings/admin.py:282 fleetpings/models.py:450
 msgid "Webhook URL"
 msgstr ""
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: fleetpings/apps.py:21
 #, python-brace-format
 msgid "Fleet Pings v{__version__}"
 msgstr ""
 
-#: fleetpings/form.py:27
+#: fleetpings/form.py:25
 msgid "Discord Markdown"
 msgstr ""
 
-#: fleetpings/form.py:34
+#: fleetpings/form.py:32
 #, python-brace-format
 msgid "Hint: You can use {discord_markdown_link} to format the text."
 msgstr ""
 
-#: fleetpings/form.py:78
+#: fleetpings/form.py:76
 msgid "Who do you want to ping?"
 msgstr ""
 
-#: fleetpings/form.py:83
+#: fleetpings/form.py:81
 msgid "Pre-Ping"
 msgstr ""
 
-#: fleetpings/form.py:84
+#: fleetpings/form.py:82
 msgid "Mark this checkbox if this should be a pre-ping."
 msgstr ""
 
-#: fleetpings/form.py:88
+#: fleetpings/form.py:86
 msgid "Ping to"
 msgstr ""
 
-#: fleetpings/form.py:90
+#: fleetpings/form.py:88
 msgid "Select a channel to ping automatically."
 msgstr ""
 
-#: fleetpings/form.py:97
+#: fleetpings/form.py:95
 msgid "FC name"
 msgstr ""
 
-#: fleetpings/form.py:99
+#: fleetpings/form.py:97
 msgid "Who is the FC?"
 msgstr ""
 
-#: fleetpings/form.py:103
+#: fleetpings/form.py:101
 msgid "Fleet name"
 msgstr ""
 
-#: fleetpings/form.py:107
+#: fleetpings/form.py:105
 msgid "What is the fleet name in the fleet finder in Eve?"
 msgstr ""
 
-#: fleetpings/form.py:113 fleetpings/models.py:305
+#: fleetpings/form.py:111 fleetpings/models.py:269
 msgid "Formup location"
 msgstr ""
 
-#: fleetpings/form.py:120
+#: fleetpings/form.py:118
 msgid "Formup time"
 msgstr ""
 
-#: fleetpings/form.py:124
+#: fleetpings/form.py:122
 msgid ""
 "To enable this field, either make it a pre-ping (checkbox above) or uncheck "
 "\"Formup NOW\" (checkbox below)."
 msgstr ""
 
-#: fleetpings/form.py:130
+#: fleetpings/form.py:128
 msgid "Formup timestamp"
 msgstr ""
 
-#: fleetpings/form.py:136
+#: fleetpings/form.py:134
 msgid "Formup NOW"
 msgstr ""
 
-#: fleetpings/form.py:138
+#: fleetpings/form.py:136
 msgid ""
 "If this checkbox is active, formup time will be set to \"NOW\" and the time "
 "in the field above (if any is set) will be ignored."
 msgstr ""
 
-#: fleetpings/form.py:144 fleetpings/models.py:168
+#: fleetpings/form.py:142 fleetpings/models.py:148
 msgid "Fleet comms"
 msgstr ""
 
-#: fleetpings/form.py:163
+#: fleetpings/form.py:161
 msgid "Webhook embed color"
 msgstr ""
 
-#: fleetpings/form.py:169
+#: fleetpings/form.py:167
 msgid "SRP"
 msgstr ""
 
-#: fleetpings/form.py:170
+#: fleetpings/form.py:168
 msgid "Is this fleet covered by SRP?"
 msgstr ""
 
-#: fleetpings/form.py:175
+#: fleetpings/form.py:173
 msgid "Create SRP link"
 msgstr ""
 
-#: fleetpings/form.py:177
+#: fleetpings/form.py:175
 msgid ""
 "If this checkbox is active, a SRP link specific for this fleet will be "
 "created.<br>Leave blank if unsure."
 msgstr ""
 
-#: fleetpings/form.py:183
+#: fleetpings/form.py:181
 msgid "Additional information"
 msgstr ""
 
-#: fleetpings/form.py:190
+#: fleetpings/form.py:188
 msgid "Feel free to add some more information about the fleet …"
 msgstr ""
 
-#: fleetpings/form.py:199
+#: fleetpings/form.py:197
 msgid "Create Optimer"
 msgstr ""
 
-#: fleetpings/form.py:201
+#: fleetpings/form.py:199
 msgid ""
 "If this checkbox is active, a fleet operations timer for this pre-ping will "
 "be created."
 msgstr ""
 
-#: fleetpings/models.py:41
+#: fleetpings/models.py:40
 msgid "You might want to install the Discord service first …"
 msgstr ""
 
-#: fleetpings/models.py:49
+#: fleetpings/models.py:47
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
 
-#: fleetpings/models.py:55
+#: fleetpings/models.py:51
 msgid "This group has not been synced to Discord yet."
 msgstr ""
 
-#: fleetpings/models.py:117
+#: fleetpings/models.py:104
 msgid "Can access this app"
 msgstr ""
 
-#: fleetpings/models.py:127
+#: fleetpings/models.py:114
 msgid "Short name to identify this comms"
 msgstr ""
 
-#: fleetpings/models.py:128 fleetpings/models.py:184 fleetpings/models.py:272
-#: fleetpings/models.py:434
+#: fleetpings/models.py:115 fleetpings/models.py:164 fleetpings/models.py:242
+#: fleetpings/models.py:378
 msgid "Name"
 msgstr ""
 
-#: fleetpings/models.py:134
+#: fleetpings/models.py:121
 msgid "In which channel is the fleet?"
 msgstr ""
 
-#: fleetpings/models.py:135
+#: fleetpings/models.py:122
 msgid "Channel"
 msgstr ""
 
-#: fleetpings/models.py:141 fleetpings/models.py:208 fleetpings/models.py:279
-#: fleetpings/models.py:351 fleetpings/models.py:458
+#: fleetpings/models.py:128 fleetpings/models.py:188 fleetpings/models.py:249
+#: fleetpings/models.py:315 fleetpings/models.py:402
 msgid "You can add notes about this configuration here if you want"
 msgstr ""
 
-#: fleetpings/models.py:142 fleetpings/models.py:209 fleetpings/models.py:280
-#: fleetpings/models.py:352 fleetpings/models.py:459 fleetpings/models.py:530
+#: fleetpings/models.py:129 fleetpings/models.py:189 fleetpings/models.py:250
+#: fleetpings/models.py:316 fleetpings/models.py:403 fleetpings/models.py:467
 msgid "Notes"
 msgstr ""
 
-#: fleetpings/models.py:148
+#: fleetpings/models.py:135
 msgid "Whether this comms is enabled or not"
 msgstr ""
 
-#: fleetpings/models.py:149 fleetpings/models.py:217 fleetpings/models.py:288
-#: fleetpings/models.py:360 fleetpings/models.py:467 fleetpings/models.py:538
+#: fleetpings/models.py:136 fleetpings/models.py:197 fleetpings/models.py:258
+#: fleetpings/models.py:324 fleetpings/models.py:411 fleetpings/models.py:475
 msgid "Is enabled"
 msgstr ""
 
-#: fleetpings/models.py:183
+#: fleetpings/models.py:163
 msgid "Short name to identify this doctrine"
 msgstr ""
 
-#: fleetpings/models.py:191
+#: fleetpings/models.py:171
 msgid "A link to a doctrine page for this doctrine if you have."
 msgstr ""
 
-#: fleetpings/models.py:200
+#: fleetpings/models.py:180
 msgid "Restrict this doctrine to the following groups …"
 msgstr ""
 
-#: fleetpings/models.py:216
+#: fleetpings/models.py:196
 msgid "Whether this doctrine is enabled or not"
 msgstr ""
 
-#: fleetpings/models.py:237
+#: fleetpings/models.py:214
 msgid "Your doctrine URL is not valid."
 msgstr ""
 
-#: fleetpings/models.py:257
+#: fleetpings/models.py:227
 msgid "Fleet doctrine"
 msgstr ""
 
-#: fleetpings/models.py:258
+#: fleetpings/models.py:228
 msgid "Fleet doctrines"
 msgstr ""
 
-#: fleetpings/models.py:271
+#: fleetpings/models.py:241
 msgid "Short name to identify this formup location"
 msgstr ""
 
-#: fleetpings/models.py:287 fleetpings/models.py:359
+#: fleetpings/models.py:257 fleetpings/models.py:323
 msgid "Whether this formup location is enabled or not"
 msgstr ""
 
-#: fleetpings/models.py:306
+#: fleetpings/models.py:270
 msgid "Formup locations"
 msgstr ""
 
-#: fleetpings/models.py:322
+#: fleetpings/models.py:286
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 
-#: fleetpings/models.py:326
+#: fleetpings/models.py:290
 msgid "Group name"
 msgstr ""
 
-#: fleetpings/models.py:334
+#: fleetpings/models.py:298
 msgid "ID of the Discord role to ping"
 msgstr ""
 
-#: fleetpings/models.py:335
+#: fleetpings/models.py:299
 msgid "Discord ID"
 msgstr ""
 
-#: fleetpings/models.py:343 fleetpings/models.py:521
+#: fleetpings/models.py:307 fleetpings/models.py:458
 msgid "Restrict ping rights to the following groups …"
 msgstr ""
 
-#: fleetpings/models.py:419
+#: fleetpings/models.py:363
 msgid "Discord ping target"
 msgstr ""
 
-#: fleetpings/models.py:420
+#: fleetpings/models.py:364
 msgid "Discord ping targets"
 msgstr ""
 
-#: fleetpings/models.py:433
+#: fleetpings/models.py:377
 msgid "Short name to identify this fleet type"
 msgstr ""
 
-#: fleetpings/models.py:441
+#: fleetpings/models.py:385
 msgid "Highlight color for the embed"
 msgstr ""
 
-#: fleetpings/models.py:450
+#: fleetpings/models.py:394
 msgid "Restrict this fleet type to the following groups …"
 msgstr ""
 
-#: fleetpings/models.py:466
+#: fleetpings/models.py:410
 msgid "Whether this fleet type is enabled or not"
 msgstr ""
 
-#: fleetpings/models.py:486
+#: fleetpings/models.py:423
 msgid "Fleet types"
 msgstr ""
 
-#: fleetpings/models.py:499
+#: fleetpings/models.py:436
 msgid "Name of the channel this webhook posts to"
 msgstr ""
 
-#: fleetpings/models.py:509
+#: fleetpings/models.py:446
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
 
-#: fleetpings/models.py:529
+#: fleetpings/models.py:466
 msgid "You can add notes about this webhook here if you want"
 msgstr ""
 
-#: fleetpings/models.py:537
+#: fleetpings/models.py:474
 msgid "Whether this webhook is active or not"
 msgstr ""
 
-#: fleetpings/models.py:556
+#: fleetpings/models.py:486
 msgid "Webhook"
 msgstr ""
 
-#: fleetpings/models.py:557
+#: fleetpings/models.py:487
 msgid "Webhooks"
 msgstr ""
 
-#: fleetpings/models.py:576
+#: fleetpings/models.py:502
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 
-#: fleetpings/models.py:596
+#: fleetpings/models.py:522
 msgid "Use default fleet types"
 msgstr ""
 
-#: fleetpings/models.py:599
+#: fleetpings/models.py:525
 msgid "Use default ping targets"
 msgstr ""
 
-#: fleetpings/models.py:602
+#: fleetpings/models.py:528
 msgid "Use Doctrines from Fittings module"
 msgstr ""
 
-#: fleetpings/models.py:604
+#: fleetpings/models.py:530
 msgid "Verify webhooks"
 msgstr ""
 
-#: fleetpings/models.py:605
+#: fleetpings/models.py:531
 msgid "Default embed color"
 msgstr ""
 
-#: fleetpings/models.py:611
+#: fleetpings/models.py:537
 msgid ""
 "Whether to use default fleet types. If checked, the default fleet types "
 "(Roaming, Home Defense, StratOP, and CTA) will be added to the Fleet Type "
 "dropdown."
 msgstr ""
 
-#: fleetpings/models.py:622
+#: fleetpings/models.py:548
 msgid ""
 "Whether to use default ping targets. If checked, the default ping targets "
 "(@everyone and @here) will be added to the Ping Target dropdown."
 msgstr ""
 
-#: fleetpings/models.py:632
+#: fleetpings/models.py:558
 msgid ""
 "Whether to use the doctrines from the Fittings modules in the doctrine "
 "dropdown. Note: The fittings module needs to be installed for this."
 msgstr ""
 
-#: fleetpings/models.py:642
+#: fleetpings/models.py:568
 msgid ""
 "Whether to verify webhooks URLs or not. Note: When unchecked, webhook URLs "
 "will not be verified, so the app can be used with non-Discord webhooks as "
 "well. When disabling webhook verification and using non-Discord webhooks, it "
 "is up to you to make sure your webhook understands a payload that is "
 "formatted for Discord webhooks."
 msgstr ""
 
-#: fleetpings/models.py:655
+#: fleetpings/models.py:581
 msgid "Default highlight color for the webhook embed."
 msgstr ""
 
-#: fleetpings/models.py:667
+#: fleetpings/models.py:593
 msgid "Setting"
 msgstr ""
 
-#: fleetpings/models.py:668
+#: fleetpings/models.py:594
 msgid "Settings"
 msgstr ""
 
-#: fleetpings/models.py:678
+#: fleetpings/models.py:597
 msgid "Fleet Pings Settings"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/index.html:11
 msgid "Fleet information"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/index.html:23
+#: fleetpings/templates/fleetpings/index.html:22
 msgid "Formatted ping text"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/index.html:51
+#: fleetpings/templates/fleetpings/index.html:49
 msgid ""
 "Mandatory information is missing. To create an optimer, you need to provide "
 "all of the following information:<br>» FC name<br>» Fleet name<br>» Formup "
 "location<br>» Formup time<br>» Ships / Doctrine"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/index.html:56
+#: fleetpings/templates/fleetpings/index.html:54
 msgid ""
 "Mandatory information is missing. To create an SRP link, you need to provide "
 "all of the following information:<br>» Fleet name<br>» Ships / Doctrine"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/index.html:60
+#: fleetpings/templates/fleetpings/index.html:58
 msgid ""
 "Error! Your ping was not copied to your clipboard. Maybe your browser "
 "doesn&apos;t support this feature."
 msgstr ""
 
-#: fleetpings/templates/fleetpings/index.html:61
+#: fleetpings/templates/fleetpings/index.html:59
 msgid ""
 "Success! Your ping text has been copied to your clipboard. Now be a good FC "
 "and throw it in your chat so you actually get some people in fleet."
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:5
 msgid ""
@@ -461,42 +461,42 @@
 "existing translation?"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/form.html:69
+#: fleetpings/templates/fleetpings/partials/form/form.html:68
 msgid "Create ping"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:6
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:7
 msgid "Please think twice if you really need to ping <code>@everyone</code>."
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:10
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:11
 msgid ""
 "\n"
-"                <code>@everyone</code>\n"
-"                includes also all the people in this channel who are offline "
-"and\n"
-"                possibly asleep at the moment and might be waking up when "
-"their\n"
-"                mobile devices ping. Or they wake up hours later to "
+"                    <code>@everyone</code>\n"
+"                    includes also all the people in this channel who are "
+"offline and\n"
+"                    possibly asleep at the moment and might be waking up "
+"when their\n"
+"                    mobile devices ping. Or they wake up hours later to "
 "irrelevant\n"
-"                pings by the time they open Discord.\n"
-"            "
+"                    pings by the time they open Discord.\n"
+"                "
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:20
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:21
 msgid ""
 "Notification spam is a real thing and might entice people to mute channels."
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:24
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:25
 msgid "<code>@here</code> usually does the trick just fine."
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/form/segments/fleet-type.html:3
 msgid "Please select"
 msgstr ""
 
@@ -536,26 +536,26 @@
 msgid "No ping created yet …"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/ping/ping.html:22
 msgid "Copy ping text"
 msgstr ""
 
-#: fleetpings/views.py:439
+#: fleetpings/views.py:394
 msgid "Not all mandatory information available to create an SRP link."
 msgstr ""
 
-#: fleetpings/views.py:474
+#: fleetpings/views.py:426
 msgid "Fleet operations timer has been created …"
 msgstr ""
 
-#: fleetpings/views.py:483
+#: fleetpings/views.py:435
 msgid "SRP link has been created …"
 msgstr ""
 
-#: fleetpings/views.py:500
+#: fleetpings/views.py:452
 msgid "Form invalid. Please check your input."
 msgstr ""
 
-#: fleetpings/views.py:502
+#: fleetpings/views.py:454
 msgid "No form data submitted."
 msgstr ""
```

### Comparing `aa_fleetpings-3.0.0/fleetpings/locale/ja/LC_MESSAGES/django.po` & `aa_fleetpings-3.0.0b1/fleetpings/locale/it_IT/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -3,457 +3,457 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-15 21:21+0100\n"
+"POT-Creation-Date: 2023-10-01 17:17+0200\n"
 "PO-Revision-Date: 2023-09-24 13:14+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-fleetpings/ja/>\n"
-"Language: ja\n"
+"Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-fleetpings/it/>\n"
+"Language: it_IT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 5.0.2\n"
 
-#: fleetpings/__init__.py:10 fleetpings/templates/fleetpings/base.html:6
+#: fleetpings/__init__.py:12 fleetpings/templates/fleetpings/base.html:5
 #: fleetpings/templates/fleetpings/base.html:10
 msgid "Fleet Pings"
 msgstr ""
 
-#: fleetpings/admin.py:114 fleetpings/models.py:167
+#: fleetpings/admin.py:104 fleetpings/models.py:147
 msgid "Fleet comm"
 msgstr ""
 
-#: fleetpings/admin.py:144 fleetpings/form.py:151
+#: fleetpings/admin.py:125 fleetpings/form.py:149
 msgid "Doctrine"
 msgstr ""
 
-#: fleetpings/admin.py:158 fleetpings/form.py:158 fleetpings/models.py:192
+#: fleetpings/admin.py:130 fleetpings/form.py:156 fleetpings/models.py:172
 msgid "Doctrine link"
 msgstr ""
 
-#: fleetpings/admin.py:173 fleetpings/admin.py:244 fleetpings/admin.py:325
-#: fleetpings/admin.py:370 fleetpings/models.py:201 fleetpings/models.py:344
-#: fleetpings/models.py:451 fleetpings/models.py:522
+#: fleetpings/admin.py:136 fleetpings/admin.py:189 fleetpings/admin.py:243
+#: fleetpings/admin.py:288 fleetpings/models.py:181 fleetpings/models.py:308
+#: fleetpings/models.py:395 fleetpings/models.py:459
 msgid "Group restrictions"
 msgstr ""
 
-#: fleetpings/admin.py:229 fleetpings/form.py:76
+#: fleetpings/admin.py:183 fleetpings/form.py:74
 msgid "Ping target"
 msgstr ""
 
-#: fleetpings/admin.py:289 fleetpings/form.py:93 fleetpings/models.py:485
+#: fleetpings/admin.py:225 fleetpings/form.py:91 fleetpings/models.py:422
 msgid "Fleet type"
 msgstr ""
 
-#: fleetpings/admin.py:303 fleetpings/models.py:442
+#: fleetpings/admin.py:230 fleetpings/models.py:386
 msgid "Embed color"
 msgstr ""
 
-#: fleetpings/admin.py:359 fleetpings/models.py:500
+#: fleetpings/admin.py:277 fleetpings/models.py:437
 msgid "Discord channel"
 msgstr ""
 
-#: fleetpings/admin.py:364 fleetpings/models.py:513
+#: fleetpings/admin.py:282 fleetpings/models.py:450
 msgid "Webhook URL"
 msgstr ""
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: fleetpings/apps.py:21
 #, python-brace-format
 msgid "Fleet Pings v{__version__}"
 msgstr ""
 
-#: fleetpings/form.py:27
+#: fleetpings/form.py:25
 msgid "Discord Markdown"
 msgstr ""
 
-#: fleetpings/form.py:34
+#: fleetpings/form.py:32
 #, python-brace-format
 msgid "Hint: You can use {discord_markdown_link} to format the text."
 msgstr ""
 
-#: fleetpings/form.py:78
+#: fleetpings/form.py:76
 msgid "Who do you want to ping?"
 msgstr ""
 
-#: fleetpings/form.py:83
+#: fleetpings/form.py:81
 msgid "Pre-Ping"
 msgstr ""
 
-#: fleetpings/form.py:84
+#: fleetpings/form.py:82
 msgid "Mark this checkbox if this should be a pre-ping."
 msgstr ""
 
-#: fleetpings/form.py:88
+#: fleetpings/form.py:86
 msgid "Ping to"
 msgstr ""
 
-#: fleetpings/form.py:90
+#: fleetpings/form.py:88
 msgid "Select a channel to ping automatically."
 msgstr ""
 
-#: fleetpings/form.py:97
+#: fleetpings/form.py:95
 msgid "FC name"
 msgstr ""
 
-#: fleetpings/form.py:99
+#: fleetpings/form.py:97
 msgid "Who is the FC?"
 msgstr ""
 
-#: fleetpings/form.py:103
+#: fleetpings/form.py:101
 msgid "Fleet name"
 msgstr ""
 
-#: fleetpings/form.py:107
+#: fleetpings/form.py:105
 msgid "What is the fleet name in the fleet finder in Eve?"
 msgstr ""
 
-#: fleetpings/form.py:113 fleetpings/models.py:305
+#: fleetpings/form.py:111 fleetpings/models.py:269
 msgid "Formup location"
 msgstr ""
 
-#: fleetpings/form.py:120
+#: fleetpings/form.py:118
 msgid "Formup time"
 msgstr ""
 
-#: fleetpings/form.py:124
+#: fleetpings/form.py:122
 msgid ""
 "To enable this field, either make it a pre-ping (checkbox above) or uncheck "
 "\"Formup NOW\" (checkbox below)."
 msgstr ""
 
-#: fleetpings/form.py:130
+#: fleetpings/form.py:128
 msgid "Formup timestamp"
 msgstr ""
 
-#: fleetpings/form.py:136
+#: fleetpings/form.py:134
 msgid "Formup NOW"
 msgstr ""
 
-#: fleetpings/form.py:138
+#: fleetpings/form.py:136
 msgid ""
 "If this checkbox is active, formup time will be set to \"NOW\" and the time "
 "in the field above (if any is set) will be ignored."
 msgstr ""
 
-#: fleetpings/form.py:144 fleetpings/models.py:168
+#: fleetpings/form.py:142 fleetpings/models.py:148
 msgid "Fleet comms"
 msgstr ""
 
-#: fleetpings/form.py:163
+#: fleetpings/form.py:161
 msgid "Webhook embed color"
 msgstr ""
 
-#: fleetpings/form.py:169
+#: fleetpings/form.py:167
 msgid "SRP"
 msgstr ""
 
-#: fleetpings/form.py:170
+#: fleetpings/form.py:168
 msgid "Is this fleet covered by SRP?"
 msgstr ""
 
-#: fleetpings/form.py:175
+#: fleetpings/form.py:173
 msgid "Create SRP link"
 msgstr ""
 
-#: fleetpings/form.py:177
+#: fleetpings/form.py:175
 msgid ""
 "If this checkbox is active, a SRP link specific for this fleet will be "
 "created.<br>Leave blank if unsure."
 msgstr ""
 
-#: fleetpings/form.py:183
+#: fleetpings/form.py:181
 msgid "Additional information"
 msgstr ""
 
-#: fleetpings/form.py:190
+#: fleetpings/form.py:188
 msgid "Feel free to add some more information about the fleet …"
 msgstr ""
 
-#: fleetpings/form.py:199
+#: fleetpings/form.py:197
 msgid "Create Optimer"
 msgstr ""
 
-#: fleetpings/form.py:201
+#: fleetpings/form.py:199
 msgid ""
 "If this checkbox is active, a fleet operations timer for this pre-ping will "
 "be created."
 msgstr ""
 
-#: fleetpings/models.py:41
+#: fleetpings/models.py:40
 msgid "You might want to install the Discord service first …"
 msgstr ""
 
-#: fleetpings/models.py:49
+#: fleetpings/models.py:47
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
 
-#: fleetpings/models.py:55
+#: fleetpings/models.py:51
 msgid "This group has not been synced to Discord yet."
 msgstr ""
 
-#: fleetpings/models.py:117
+#: fleetpings/models.py:104
 msgid "Can access this app"
 msgstr ""
 
-#: fleetpings/models.py:127
+#: fleetpings/models.py:114
 msgid "Short name to identify this comms"
 msgstr ""
 
-#: fleetpings/models.py:128 fleetpings/models.py:184 fleetpings/models.py:272
-#: fleetpings/models.py:434
+#: fleetpings/models.py:115 fleetpings/models.py:164 fleetpings/models.py:242
+#: fleetpings/models.py:378
 msgid "Name"
 msgstr ""
 
-#: fleetpings/models.py:134
+#: fleetpings/models.py:121
 msgid "In which channel is the fleet?"
 msgstr ""
 
-#: fleetpings/models.py:135
+#: fleetpings/models.py:122
 msgid "Channel"
 msgstr ""
 
-#: fleetpings/models.py:141 fleetpings/models.py:208 fleetpings/models.py:279
-#: fleetpings/models.py:351 fleetpings/models.py:458
+#: fleetpings/models.py:128 fleetpings/models.py:188 fleetpings/models.py:249
+#: fleetpings/models.py:315 fleetpings/models.py:402
 msgid "You can add notes about this configuration here if you want"
 msgstr ""
 
-#: fleetpings/models.py:142 fleetpings/models.py:209 fleetpings/models.py:280
-#: fleetpings/models.py:352 fleetpings/models.py:459 fleetpings/models.py:530
+#: fleetpings/models.py:129 fleetpings/models.py:189 fleetpings/models.py:250
+#: fleetpings/models.py:316 fleetpings/models.py:403 fleetpings/models.py:467
 msgid "Notes"
 msgstr ""
 
-#: fleetpings/models.py:148
+#: fleetpings/models.py:135
 msgid "Whether this comms is enabled or not"
 msgstr ""
 
-#: fleetpings/models.py:149 fleetpings/models.py:217 fleetpings/models.py:288
-#: fleetpings/models.py:360 fleetpings/models.py:467 fleetpings/models.py:538
+#: fleetpings/models.py:136 fleetpings/models.py:197 fleetpings/models.py:258
+#: fleetpings/models.py:324 fleetpings/models.py:411 fleetpings/models.py:475
 msgid "Is enabled"
 msgstr ""
 
-#: fleetpings/models.py:183
+#: fleetpings/models.py:163
 msgid "Short name to identify this doctrine"
 msgstr ""
 
-#: fleetpings/models.py:191
+#: fleetpings/models.py:171
 msgid "A link to a doctrine page for this doctrine if you have."
 msgstr ""
 
-#: fleetpings/models.py:200
+#: fleetpings/models.py:180
 msgid "Restrict this doctrine to the following groups …"
 msgstr ""
 
-#: fleetpings/models.py:216
+#: fleetpings/models.py:196
 msgid "Whether this doctrine is enabled or not"
 msgstr ""
 
-#: fleetpings/models.py:237
+#: fleetpings/models.py:214
 msgid "Your doctrine URL is not valid."
 msgstr ""
 
-#: fleetpings/models.py:257
+#: fleetpings/models.py:227
 msgid "Fleet doctrine"
 msgstr ""
 
-#: fleetpings/models.py:258
+#: fleetpings/models.py:228
 msgid "Fleet doctrines"
 msgstr ""
 
-#: fleetpings/models.py:271
+#: fleetpings/models.py:241
 msgid "Short name to identify this formup location"
 msgstr ""
 
-#: fleetpings/models.py:287 fleetpings/models.py:359
+#: fleetpings/models.py:257 fleetpings/models.py:323
 msgid "Whether this formup location is enabled or not"
 msgstr ""
 
-#: fleetpings/models.py:306
+#: fleetpings/models.py:270
 msgid "Formup locations"
 msgstr ""
 
-#: fleetpings/models.py:322
+#: fleetpings/models.py:286
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 
-#: fleetpings/models.py:326
+#: fleetpings/models.py:290
 msgid "Group name"
 msgstr ""
 
-#: fleetpings/models.py:334
+#: fleetpings/models.py:298
 msgid "ID of the Discord role to ping"
 msgstr ""
 
-#: fleetpings/models.py:335
+#: fleetpings/models.py:299
 msgid "Discord ID"
 msgstr ""
 
-#: fleetpings/models.py:343 fleetpings/models.py:521
+#: fleetpings/models.py:307 fleetpings/models.py:458
 msgid "Restrict ping rights to the following groups …"
 msgstr ""
 
-#: fleetpings/models.py:419
+#: fleetpings/models.py:363
 msgid "Discord ping target"
 msgstr ""
 
-#: fleetpings/models.py:420
+#: fleetpings/models.py:364
 msgid "Discord ping targets"
 msgstr ""
 
-#: fleetpings/models.py:433
+#: fleetpings/models.py:377
 msgid "Short name to identify this fleet type"
 msgstr ""
 
-#: fleetpings/models.py:441
+#: fleetpings/models.py:385
 msgid "Highlight color for the embed"
 msgstr ""
 
-#: fleetpings/models.py:450
+#: fleetpings/models.py:394
 msgid "Restrict this fleet type to the following groups …"
 msgstr ""
 
-#: fleetpings/models.py:466
+#: fleetpings/models.py:410
 msgid "Whether this fleet type is enabled or not"
 msgstr ""
 
-#: fleetpings/models.py:486
+#: fleetpings/models.py:423
 msgid "Fleet types"
 msgstr ""
 
-#: fleetpings/models.py:499
+#: fleetpings/models.py:436
 msgid "Name of the channel this webhook posts to"
 msgstr ""
 
-#: fleetpings/models.py:509
+#: fleetpings/models.py:446
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
 
-#: fleetpings/models.py:529
+#: fleetpings/models.py:466
 msgid "You can add notes about this webhook here if you want"
 msgstr ""
 
-#: fleetpings/models.py:537
+#: fleetpings/models.py:474
 msgid "Whether this webhook is active or not"
 msgstr ""
 
-#: fleetpings/models.py:556
+#: fleetpings/models.py:486
 msgid "Webhook"
 msgstr ""
 
-#: fleetpings/models.py:557
+#: fleetpings/models.py:487
 msgid "Webhooks"
 msgstr ""
 
-#: fleetpings/models.py:576
+#: fleetpings/models.py:502
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 
-#: fleetpings/models.py:596
+#: fleetpings/models.py:522
 msgid "Use default fleet types"
 msgstr ""
 
-#: fleetpings/models.py:599
+#: fleetpings/models.py:525
 msgid "Use default ping targets"
 msgstr ""
 
-#: fleetpings/models.py:602
+#: fleetpings/models.py:528
 msgid "Use Doctrines from Fittings module"
 msgstr ""
 
-#: fleetpings/models.py:604
+#: fleetpings/models.py:530
 msgid "Verify webhooks"
 msgstr ""
 
-#: fleetpings/models.py:605
+#: fleetpings/models.py:531
 msgid "Default embed color"
 msgstr ""
 
-#: fleetpings/models.py:611
+#: fleetpings/models.py:537
 msgid ""
 "Whether to use default fleet types. If checked, the default fleet types "
 "(Roaming, Home Defense, StratOP, and CTA) will be added to the Fleet Type "
 "dropdown."
 msgstr ""
 
-#: fleetpings/models.py:622
+#: fleetpings/models.py:548
 msgid ""
 "Whether to use default ping targets. If checked, the default ping targets "
 "(@everyone and @here) will be added to the Ping Target dropdown."
 msgstr ""
 
-#: fleetpings/models.py:632
+#: fleetpings/models.py:558
 msgid ""
 "Whether to use the doctrines from the Fittings modules in the doctrine "
 "dropdown. Note: The fittings module needs to be installed for this."
 msgstr ""
 
-#: fleetpings/models.py:642
+#: fleetpings/models.py:568
 msgid ""
 "Whether to verify webhooks URLs or not. Note: When unchecked, webhook URLs "
 "will not be verified, so the app can be used with non-Discord webhooks as "
 "well. When disabling webhook verification and using non-Discord webhooks, it "
 "is up to you to make sure your webhook understands a payload that is "
 "formatted for Discord webhooks."
 msgstr ""
 
-#: fleetpings/models.py:655
+#: fleetpings/models.py:581
 msgid "Default highlight color for the webhook embed."
 msgstr ""
 
-#: fleetpings/models.py:667
+#: fleetpings/models.py:593
 msgid "Setting"
 msgstr ""
 
-#: fleetpings/models.py:668
+#: fleetpings/models.py:594
 msgid "Settings"
 msgstr ""
 
-#: fleetpings/models.py:678
+#: fleetpings/models.py:597
 msgid "Fleet Pings Settings"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/index.html:11
 msgid "Fleet information"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/index.html:23
+#: fleetpings/templates/fleetpings/index.html:22
 msgid "Formatted ping text"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/index.html:51
+#: fleetpings/templates/fleetpings/index.html:49
 msgid ""
 "Mandatory information is missing. To create an optimer, you need to provide "
 "all of the following information:<br>» FC name<br>» Fleet name<br>» Formup "
 "location<br>» Formup time<br>» Ships / Doctrine"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/index.html:56
+#: fleetpings/templates/fleetpings/index.html:54
 msgid ""
 "Mandatory information is missing. To create an SRP link, you need to provide "
 "all of the following information:<br>» Fleet name<br>» Ships / Doctrine"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/index.html:60
+#: fleetpings/templates/fleetpings/index.html:58
 msgid ""
 "Error! Your ping was not copied to your clipboard. Maybe your browser "
 "doesn&apos;t support this feature."
 msgstr ""
 
-#: fleetpings/templates/fleetpings/index.html:61
+#: fleetpings/templates/fleetpings/index.html:59
 msgid ""
 "Success! Your ping text has been copied to your clipboard. Now be a good FC "
 "and throw it in your chat so you actually get some people in fleet."
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:5
 msgid ""
@@ -461,42 +461,42 @@
 "existing translation?"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/form.html:69
+#: fleetpings/templates/fleetpings/partials/form/form.html:68
 msgid "Create ping"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:6
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:7
 msgid "Please think twice if you really need to ping <code>@everyone</code>."
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:10
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:11
 msgid ""
 "\n"
-"                <code>@everyone</code>\n"
-"                includes also all the people in this channel who are offline "
-"and\n"
-"                possibly asleep at the moment and might be waking up when "
-"their\n"
-"                mobile devices ping. Or they wake up hours later to "
+"                    <code>@everyone</code>\n"
+"                    includes also all the people in this channel who are "
+"offline and\n"
+"                    possibly asleep at the moment and might be waking up "
+"when their\n"
+"                    mobile devices ping. Or they wake up hours later to "
 "irrelevant\n"
-"                pings by the time they open Discord.\n"
-"            "
+"                    pings by the time they open Discord.\n"
+"                "
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:20
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:21
 msgid ""
 "Notification spam is a real thing and might entice people to mute channels."
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:24
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:25
 msgid "<code>@here</code> usually does the trick just fine."
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/form/segments/fleet-type.html:3
 msgid "Please select"
 msgstr ""
 
@@ -536,26 +536,26 @@
 msgid "No ping created yet …"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/ping/ping.html:22
 msgid "Copy ping text"
 msgstr ""
 
-#: fleetpings/views.py:439
+#: fleetpings/views.py:394
 msgid "Not all mandatory information available to create an SRP link."
 msgstr ""
 
-#: fleetpings/views.py:474
+#: fleetpings/views.py:426
 msgid "Fleet operations timer has been created …"
 msgstr ""
 
-#: fleetpings/views.py:483
+#: fleetpings/views.py:435
 msgid "SRP link has been created …"
 msgstr ""
 
-#: fleetpings/views.py:500
+#: fleetpings/views.py:452
 msgid "Form invalid. Please check your input."
 msgstr ""
 
-#: fleetpings/views.py:502
+#: fleetpings/views.py:454
 msgid "No form data submitted."
 msgstr ""
```

### Comparing `aa_fleetpings-3.0.0/fleetpings/locale/ko_KR/LC_MESSAGES/django.mo` & `aa_fleetpings-3.0.0b1/fleetpings/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/locale/ko_KR/LC_MESSAGES/django.po` & `aa_fleetpings-3.0.0b1/fleetpings/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,455 +3,453 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Author50CO <tkddlschry@gmail.com>, 2023.
 # Peter Pfeufer <info@ppfeufer.de>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-15 21:21+0100\n"
+"POT-Creation-Date: 2023-10-01 17:17+0200\n"
 "PO-Revision-Date: 2023-12-29 09:04+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Korean <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-fleetpings/ko/>\n"
+"Language-Team: Korean <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-fleetpings/ko/>\n"
 "Language: ko_KR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "X-Generator: Weblate 5.3.1\n"
 
-#: fleetpings/__init__.py:10 fleetpings/templates/fleetpings/base.html:6
+#: fleetpings/__init__.py:12 fleetpings/templates/fleetpings/base.html:5
 #: fleetpings/templates/fleetpings/base.html:10
 msgid "Fleet Pings"
 msgstr "함대 핑"
 
-#: fleetpings/admin.py:114 fleetpings/models.py:167
+#: fleetpings/admin.py:104 fleetpings/models.py:147
 msgid "Fleet comm"
 msgstr "함대 음성채널"
 
-#: fleetpings/admin.py:144 fleetpings/form.py:151
+#: fleetpings/admin.py:125 fleetpings/form.py:149
 msgid "Doctrine"
 msgstr "독트린"
 
-#: fleetpings/admin.py:158 fleetpings/form.py:158 fleetpings/models.py:192
+#: fleetpings/admin.py:130 fleetpings/form.py:156 fleetpings/models.py:172
 msgid "Doctrine link"
 msgstr "독트린 링크"
 
-#: fleetpings/admin.py:173 fleetpings/admin.py:244 fleetpings/admin.py:325
-#: fleetpings/admin.py:370 fleetpings/models.py:201 fleetpings/models.py:344
-#: fleetpings/models.py:451 fleetpings/models.py:522
+#: fleetpings/admin.py:136 fleetpings/admin.py:189 fleetpings/admin.py:243
+#: fleetpings/admin.py:288 fleetpings/models.py:181 fleetpings/models.py:308
+#: fleetpings/models.py:395 fleetpings/models.py:459
 msgid "Group restrictions"
 msgstr "그룹 제한"
 
-#: fleetpings/admin.py:229 fleetpings/form.py:76
+#: fleetpings/admin.py:183 fleetpings/form.py:74
 #, fuzzy
 #| msgid "Ping Target"
 msgid "Ping target"
 msgstr "핑 역할"
 
-#: fleetpings/admin.py:289 fleetpings/form.py:93 fleetpings/models.py:485
+#: fleetpings/admin.py:225 fleetpings/form.py:91 fleetpings/models.py:422
 msgid "Fleet type"
 msgstr "함대 종류"
 
-#: fleetpings/admin.py:303 fleetpings/models.py:442
+#: fleetpings/admin.py:230 fleetpings/models.py:386
 msgid "Embed color"
 msgstr "Embed 색상"
 
-#: fleetpings/admin.py:359 fleetpings/models.py:500
+#: fleetpings/admin.py:277 fleetpings/models.py:437
 msgid "Discord channel"
 msgstr "디스코드 채널"
 
-#: fleetpings/admin.py:364 fleetpings/models.py:513
+#: fleetpings/admin.py:282 fleetpings/models.py:450
 msgid "Webhook URL"
 msgstr "웹훅 URL"
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: fleetpings/apps.py:21
 #, python-brace-format
 msgid "Fleet Pings v{__version__}"
 msgstr "플릿 핑 v{__version__}"
 
-#: fleetpings/form.py:27
+#: fleetpings/form.py:25
 msgid "Discord Markdown"
 msgstr "디스코드 마크다운"
 
-#: fleetpings/form.py:34
+#: fleetpings/form.py:32
 #, python-brace-format
 msgid "Hint: You can use {discord_markdown_link} to format the text."
 msgstr ""
 "힌트: {discord_markdown_link}를 사용해 텍스트 양식을 변경할 수 있습니다."
 
-#: fleetpings/form.py:78
+#: fleetpings/form.py:76
 msgid "Who do you want to ping?"
 msgstr "핑을 보낼까요?"
 
-#: fleetpings/form.py:83
+#: fleetpings/form.py:81
 msgid "Pre-Ping"
 msgstr "예고 핑"
 
-#: fleetpings/form.py:84
+#: fleetpings/form.py:82
 msgid "Mark this checkbox if this should be a pre-ping."
 msgstr "예고 핑인 경우 체크박스를 선택하세요."
 
-#: fleetpings/form.py:88
+#: fleetpings/form.py:86
 #, fuzzy
 #| msgid "Ping To"
 msgid "Ping to"
 msgstr "핑 보낼 대상"
 
-#: fleetpings/form.py:90
+#: fleetpings/form.py:88
 msgid "Select a channel to ping automatically."
 msgstr "자동으로 핑을 보낼 채널을 선택하세요."
 
-#: fleetpings/form.py:97
+#: fleetpings/form.py:95
 msgid "FC name"
 msgstr ""
 
-#: fleetpings/form.py:99
+#: fleetpings/form.py:97
 msgid "Who is the FC?"
 msgstr "함대 지휘관이 누구인가요?"
 
-#: fleetpings/form.py:103
+#: fleetpings/form.py:101
 #, fuzzy
 #| msgid "Fleet Name"
 msgid "Fleet name"
 msgstr "함대 이름"
 
-#: fleetpings/form.py:107
+#: fleetpings/form.py:105
 #, fuzzy
 #| msgid "What is the fleet name in fleet finder?"
 msgid "What is the fleet name in the fleet finder in Eve?"
 msgstr "함대 찾기에서 플릿 이름이 무엇인가요?"
 
-#: fleetpings/form.py:113 fleetpings/models.py:305
+#: fleetpings/form.py:111 fleetpings/models.py:269
 #, fuzzy
 #| msgid "Formup Location"
 msgid "Formup location"
 msgstr "폼업 위치"
 
-#: fleetpings/form.py:120
+#: fleetpings/form.py:118
 #, fuzzy
 #| msgid "Formup Time"
 msgid "Formup time"
 msgstr "폼업 시간"
 
-#: fleetpings/form.py:124
+#: fleetpings/form.py:122
 msgid ""
 "To enable this field, either make it a pre-ping (checkbox above) or uncheck "
 "\"Formup NOW\" (checkbox below)."
-msgstr ""
-"이 창을 활성화하려면, 예고 핑을 활성화하거나(위 체크박스), “지금 폼업하기” 체"
-"크 박스를 해제하세요."
+msgstr "이 창을 활성화하려면, 예고 핑을 활성화하거나(위 체크박스), “지금 폼업하기” "
+"체크 박스를 해제하세요."
 
-#: fleetpings/form.py:130
+#: fleetpings/form.py:128
 #, fuzzy
 #| msgid "Formup Timestamp"
 msgid "Formup timestamp"
 msgstr "폼업 타임스탬프"
 
-#: fleetpings/form.py:136
+#: fleetpings/form.py:134
 msgid "Formup NOW"
 msgstr "지금 폼업"
 
-#: fleetpings/form.py:138
+#: fleetpings/form.py:136
 msgid ""
 "If this checkbox is active, formup time will be set to \"NOW\" and the time "
 "in the field above (if any is set) will be ignored."
-msgstr ""
-"이 체크박스가 활성화되어 있으면, 폼업 시간이 “지금” 으로 설정되며 위쪽에 설정"
-"된 시간을 무시합니다."
+msgstr "이 체크박스가 활성화되어 있으면, 폼업 시간이 “지금” 으로 설정되며 위쪽에 "
+"설정된 시간을 무시합니다."
 
-#: fleetpings/form.py:144 fleetpings/models.py:168
+#: fleetpings/form.py:142 fleetpings/models.py:148
 #, fuzzy
 #| msgid "Fleet Comms"
 msgid "Fleet comms"
 msgstr "함대 음성"
 
-#: fleetpings/form.py:163
+#: fleetpings/form.py:161
 #, fuzzy
 #| msgid "Webhook Embed Color"
 msgid "Webhook embed color"
 msgstr "웹훅 Embed 색상"
 
-#: fleetpings/form.py:169
+#: fleetpings/form.py:167
 msgid "SRP"
 msgstr "SRP"
 
-#: fleetpings/form.py:170
+#: fleetpings/form.py:168
 msgid "Is this fleet covered by SRP?"
 msgstr "SRP가 가능한 함대인가요?"
 
-#: fleetpings/form.py:175
+#: fleetpings/form.py:173
 #, fuzzy
 #| msgid "Create SRP Link"
 msgid "Create SRP link"
 msgstr "SRP 주소 생성"
 
-#: fleetpings/form.py:177
+#: fleetpings/form.py:175
 msgid ""
 "If this checkbox is active, a SRP link specific for this fleet will be "
 "created.<br>Leave blank if unsure."
 msgstr ""
 "이 체크박스가 활성화되어 있으면, 이 함대에 대한 SRP 링크가 생성됩니다. <br> "
 "확실하지 않은 경우 체크하지 마세요."
 
-#: fleetpings/form.py:183
+#: fleetpings/form.py:181
 msgid "Additional information"
 msgstr "추가 정보"
 
-#: fleetpings/form.py:190
+#: fleetpings/form.py:188
 msgid "Feel free to add some more information about the fleet …"
 msgstr "함대에 대한 추가 정보를 입력하세요…"
 
-#: fleetpings/form.py:199
+#: fleetpings/form.py:197
 msgid "Create Optimer"
 msgstr "옵 타이머 생성"
 
-#: fleetpings/form.py:201
+#: fleetpings/form.py:199
 msgid ""
 "If this checkbox is active, a fleet operations timer for this pre-ping will "
 "be created."
 msgstr ""
 "이 체크박스가 활성화되어 있으면, 이 예고 핑에 대한 함대 옵 타이머가 생성됩니"
 "다."
 
-#: fleetpings/models.py:41
+#: fleetpings/models.py:40
 msgid "You might want to install the Discord service first …"
 msgstr "디스코드 서비스를 먼저 설치해주세요…"
 
-#: fleetpings/models.py:49
+#: fleetpings/models.py:47
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr "디스코드가 Alliance Auth와 연동되어 있나요?"
 
-#: fleetpings/models.py:55
+#: fleetpings/models.py:51
 msgid "This group has not been synced to Discord yet."
 msgstr "이 그룹은 아직 디스코드와 연동되어 있지 않습니다."
 
-#: fleetpings/models.py:117
+#: fleetpings/models.py:104
 msgid "Can access this app"
 msgstr "서비스에 접근할 수 있습니다"
 
-#: fleetpings/models.py:127
+#: fleetpings/models.py:114
 msgid "Short name to identify this comms"
 msgstr "함대 음성 채널 이름을 설명하는 짧은 이름"
 
-#: fleetpings/models.py:128 fleetpings/models.py:184 fleetpings/models.py:272
-#: fleetpings/models.py:434
+#: fleetpings/models.py:115 fleetpings/models.py:164 fleetpings/models.py:242
+#: fleetpings/models.py:378
 msgid "Name"
 msgstr "이름"
 
-#: fleetpings/models.py:134
+#: fleetpings/models.py:121
 msgid "In which channel is the fleet?"
 msgstr "어떤 음성 채널을 사용하나요?"
 
-#: fleetpings/models.py:135
+#: fleetpings/models.py:122
 msgid "Channel"
 msgstr "채널"
 
-#: fleetpings/models.py:141 fleetpings/models.py:208 fleetpings/models.py:279
-#: fleetpings/models.py:351 fleetpings/models.py:458
+#: fleetpings/models.py:128 fleetpings/models.py:188 fleetpings/models.py:249
+#: fleetpings/models.py:315 fleetpings/models.py:402
 msgid "You can add notes about this configuration here if you want"
 msgstr "해당 설정에 대한 설명을 남길 수 있습니다"
 
-#: fleetpings/models.py:142 fleetpings/models.py:209 fleetpings/models.py:280
-#: fleetpings/models.py:352 fleetpings/models.py:459 fleetpings/models.py:530
+#: fleetpings/models.py:129 fleetpings/models.py:189 fleetpings/models.py:250
+#: fleetpings/models.py:316 fleetpings/models.py:403 fleetpings/models.py:467
 msgid "Notes"
 msgstr "설명"
 
-#: fleetpings/models.py:148
+#: fleetpings/models.py:135
 msgid "Whether this comms is enabled or not"
 msgstr "음성 채널 활성화 및 비활성화"
 
-#: fleetpings/models.py:149 fleetpings/models.py:217 fleetpings/models.py:288
-#: fleetpings/models.py:360 fleetpings/models.py:467 fleetpings/models.py:538
+#: fleetpings/models.py:136 fleetpings/models.py:197 fleetpings/models.py:258
+#: fleetpings/models.py:324 fleetpings/models.py:411 fleetpings/models.py:475
 msgid "Is enabled"
 msgstr "활성화"
 
-#: fleetpings/models.py:183
+#: fleetpings/models.py:163
 msgid "Short name to identify this doctrine"
 msgstr "독트린 이름을 설명하는 짧은 이름"
 
-#: fleetpings/models.py:191
+#: fleetpings/models.py:171
 msgid "A link to a doctrine page for this doctrine if you have."
 msgstr "해당 독트린 페이지의 링크."
 
-#: fleetpings/models.py:200
+#: fleetpings/models.py:180
 msgid "Restrict this doctrine to the following groups …"
 msgstr "다음 그룹만 해당 독트린을 사용할 수 있습니다…"
 
-#: fleetpings/models.py:216
+#: fleetpings/models.py:196
 msgid "Whether this doctrine is enabled or not"
 msgstr "독트린 활성화 및 비활성화"
 
-#: fleetpings/models.py:237
+#: fleetpings/models.py:214
 msgid "Your doctrine URL is not valid."
 msgstr "잘못된 독트린 URL 입니다."
 
-#: fleetpings/models.py:257
+#: fleetpings/models.py:227
 #, fuzzy
 #| msgid "Fleet Doctrine"
 msgid "Fleet doctrine"
 msgstr "함대 독트린"
 
-#: fleetpings/models.py:258
+#: fleetpings/models.py:228
 #, fuzzy
 #| msgid "Fleet Doctrines"
 msgid "Fleet doctrines"
 msgstr "함대 독트린"
 
-#: fleetpings/models.py:271
+#: fleetpings/models.py:241
 msgid "Short name to identify this formup location"
 msgstr "폼업 위치 이름을 설명하는 짧은 이름"
 
-#: fleetpings/models.py:287 fleetpings/models.py:359
+#: fleetpings/models.py:257 fleetpings/models.py:323
 msgid "Whether this formup location is enabled or not"
 msgstr "폼업지 활성화 및 비활성화"
 
-#: fleetpings/models.py:306
+#: fleetpings/models.py:270
 #, fuzzy
 #| msgid "Formup Locations"
 msgid "Formup locations"
 msgstr "폼업 위치"
 
-#: fleetpings/models.py:322
+#: fleetpings/models.py:286
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 "핑을 보낼 디스코드 역할. (설명: 디스코드와 연동된 Auth 그룹이어야 합니다.)"
 
-#: fleetpings/models.py:326
+#: fleetpings/models.py:290
 msgid "Group name"
 msgstr "그룹 이름"
 
-#: fleetpings/models.py:334
+#: fleetpings/models.py:298
 msgid "ID of the Discord role to ping"
 msgstr "핑을 보낼 역할의 디스코드 역할 ID"
 
-#: fleetpings/models.py:335
+#: fleetpings/models.py:299
 msgid "Discord ID"
 msgstr "역할 ID"
 
-#: fleetpings/models.py:343 fleetpings/models.py:521
+#: fleetpings/models.py:307 fleetpings/models.py:458
 msgid "Restrict ping rights to the following groups …"
 msgstr "다음 그룹만 핑을 보낼 수 있습니다…"
 
-#: fleetpings/models.py:419
+#: fleetpings/models.py:363
 #, fuzzy
 #| msgid "Discord Ping Target"
 msgid "Discord ping target"
 msgstr "핑 보낼 디스코드 역할"
 
-#: fleetpings/models.py:420
+#: fleetpings/models.py:364
 #, fuzzy
 #| msgid "Discord Ping Targets"
 msgid "Discord ping targets"
 msgstr "핑 보낼 디스코드 역할"
 
-#: fleetpings/models.py:433
+#: fleetpings/models.py:377
 msgid "Short name to identify this fleet type"
 msgstr "함대 종류를 설명하는 짧은 이름"
 
-#: fleetpings/models.py:441
+#: fleetpings/models.py:385
 msgid "Highlight color for the embed"
 msgstr "embed의 하이라이트 색상"
 
-#: fleetpings/models.py:450
+#: fleetpings/models.py:394
 msgid "Restrict this fleet type to the following groups …"
 msgstr "다음 그룹만 이 함대 종류를 참가할 수 있습니다…"
 
-#: fleetpings/models.py:466
+#: fleetpings/models.py:410
 msgid "Whether this fleet type is enabled or not"
 msgstr "함대 종류 활성화 및 비활성화"
 
-#: fleetpings/models.py:486
+#: fleetpings/models.py:423
 msgid "Fleet types"
 msgstr "함대 종류"
 
-#: fleetpings/models.py:499
+#: fleetpings/models.py:436
 msgid "Name of the channel this webhook posts to"
 msgstr "웹훅과 연결된 채널 이름"
 
-#: fleetpings/models.py:509
+#: fleetpings/models.py:446
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr "웹훅의 URL, 예시) https://discord.com/api/webhooks/123456/abcdef"
 
-#: fleetpings/models.py:529
+#: fleetpings/models.py:466
 msgid "You can add notes about this webhook here if you want"
 msgstr "웹훅에 대한 설명을 남길 수 있습니다"
 
-#: fleetpings/models.py:537
+#: fleetpings/models.py:474
 msgid "Whether this webhook is active or not"
 msgstr "웹훅 활성화 및 비활성화"
 
-#: fleetpings/models.py:556
+#: fleetpings/models.py:486
 msgid "Webhook"
 msgstr "웹훅"
 
-#: fleetpings/models.py:557
+#: fleetpings/models.py:487
 msgid "Webhooks"
 msgstr "웹훅"
 
-#: fleetpings/models.py:576
+#: fleetpings/models.py:502
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 "잘못된 웹훅 URL. 알려진 디스코드의 웹훅 URL 형태와 일치하지 않습니다. 웹훅 "
 "URL을 확인해 주세요."
 
-#: fleetpings/models.py:596
+#: fleetpings/models.py:522
 msgid "Use default fleet types"
 msgstr "기본 함대 종류 사용"
 
-#: fleetpings/models.py:599
+#: fleetpings/models.py:525
 msgid "Use default ping targets"
 msgstr "기본 핑 역할 사용"
 
-#: fleetpings/models.py:602
+#: fleetpings/models.py:528
 msgid "Use Doctrines from Fittings module"
 msgstr "피팅 모듈에서 만들어진 독트린을 사용하세요"
 
-#: fleetpings/models.py:604
+#: fleetpings/models.py:530
 #, fuzzy
 #| msgid "Verify Webhooks"
 msgid "Verify webhooks"
 msgstr "웹훅 검사"
 
-#: fleetpings/models.py:605
+#: fleetpings/models.py:531
 msgid "Default embed color"
 msgstr "기본 embed 색상"
 
-#: fleetpings/models.py:611
+#: fleetpings/models.py:537
 msgid ""
 "Whether to use default fleet types. If checked, the default fleet types "
 "(Roaming, Home Defense, StratOP, and CTA) will be added to the Fleet Type "
 "dropdown."
 msgstr ""
 "기본 함대 종류를 사용할지 여부 설정. 활성화된 경우, 기본 함대 종류(로밍, 기"
 "지 방어, 스트랫 옵, CTA)가 함대 종류 드롭다운 메뉴에 추가됩니다."
 
-#: fleetpings/models.py:622
+#: fleetpings/models.py:548
 msgid ""
 "Whether to use default ping targets. If checked, the default ping targets "
 "(@everyone and @here) will be added to the Ping Target dropdown."
 msgstr ""
 "기본 핑 역할 사용 여부 설정. 활성화된 경우, 기본 핑 역할 (@everyone 과 "
 "@here) 가 핑 역할 드롭다운에 추가됩니다."
 
-#: fleetpings/models.py:632
+#: fleetpings/models.py:558
 msgid ""
 "Whether to use the doctrines from the Fittings modules in the doctrine "
 "dropdown. Note: The fittings module needs to be installed for this."
 msgstr ""
 "독트린 드롭다운에서 해당 독트린의 피팅 모듈 사용 여부 설정. 설명: 피팅 모듈"
 "이 설치되어 있어야 합니다."
 
-#: fleetpings/models.py:642
+#: fleetpings/models.py:568
 #, fuzzy
 #| msgid ""
 #| "Whether to verify Webhooks URLs or not. Note: When unchecked Webhook URLs "
 #| "will not be verified, so the app can be used with non-Discord Webhooks as "
 #| "well. When disabling webhook verification and using non-Discord webhooks, "
 #| "it is up to you to make sure your webhook understands a payload that is "
 #| "formatted for Discord webhooks."
@@ -463,81 +461,81 @@
 "formatted for Discord webhooks."
 msgstr ""
 "웹훅 URL을 검사할지 여부 설정. 설명: 체크가 해제되어 있을 경우 웹훅 URL을 검"
 "사하지 않습니다, 따라서 디스코드가 아닌 웹훅도 사용할 수 있습니다. 웹훅 검사"
 "를 해제하고 디스코드가 아닌 웹훅을 사용할 경우, 웹훅이 디스코드로 보내질 만큼"
 "의 payload를 감당할 수 있을지 판단은 사용자의 몫입니다."
 
-#: fleetpings/models.py:655
+#: fleetpings/models.py:581
 msgid "Default highlight color for the webhook embed."
 msgstr "웹훅 embed 기본 하이라이트 색상."
 
-#: fleetpings/models.py:667
+#: fleetpings/models.py:593
 #, fuzzy
 #| msgid "setting"
 msgid "Setting"
 msgstr "설정"
 
-#: fleetpings/models.py:668
+#: fleetpings/models.py:594
 msgid "Settings"
 msgstr "설정"
 
-#: fleetpings/models.py:678
+#: fleetpings/models.py:597
 msgid "Fleet Pings Settings"
 msgstr "함대 핑 설정"
 
 #: fleetpings/templates/fleetpings/index.html:11
 #, fuzzy
 #| msgid "Fleet Information"
 msgid "Fleet information"
 msgstr "함대 정보"
 
-#: fleetpings/templates/fleetpings/index.html:23
+#: fleetpings/templates/fleetpings/index.html:22
 #, fuzzy
 #| msgid "Formatted Ping Text"
 msgid "Formatted ping text"
 msgstr "양식 적용된 핑 텍스트"
 
-#: fleetpings/templates/fleetpings/index.html:51
+#: fleetpings/templates/fleetpings/index.html:49
 #, fuzzy
 #| msgid ""
 #| "Mandatory information is missing. To create an optimer, you need to "
 #| "provide all of the following information:<br>» FC Name<br>» Fleet "
 #| "Name<br>» Formup Location<br>» Formup Time<br>» Ships / Doctrine"
 msgid ""
 "Mandatory information is missing. To create an optimer, you need to provide "
 "all of the following information:<br>» FC name<br>» Fleet name<br>» Formup "
 "location<br>» Formup time<br>» Ships / Doctrine"
 msgstr ""
 "필수 정보가 누락되었습니다. 옵 타이머를 생성하려면, 다음 정보를 모두 제공해"
 "야 합니다:<br>» 함대 지휘관 이름<br>» 플릿 이름<br>» 폼업 지역<br>» 폼업 시각"
 "<br>» 함선/독트린"
 
-#: fleetpings/templates/fleetpings/index.html:56
+#: fleetpings/templates/fleetpings/index.html:54
 #, fuzzy
 #| msgid ""
 #| "Mandatory information is missing. To create an SRP link, you need to "
 #| "provide all of the following information:<br>» Fleet Name<br>» Ships / "
 #| "Doctrine"
 msgid ""
 "Mandatory information is missing. To create an SRP link, you need to provide "
 "all of the following information:<br>» Fleet name<br>» Ships / Doctrine"
 msgstr ""
 "필수 정보가 누락되었습니다. SRP 링크를 생성하려면, 다음 정보를 모두 제공해야 "
 "합니다:<br>» 함대 이름<br>» 함선 / 독트린"
 
-#: fleetpings/templates/fleetpings/index.html:60
+#: fleetpings/templates/fleetpings/index.html:58
 msgid ""
 "Error! Your ping was not copied to your clipboard. Maybe your browser "
 "doesn&apos;t support this feature."
 msgstr ""
 "오류! 핑이 클립보드에 복사되지 않았습니다. 브라우저가 이 기능을 지원하지 않"
 "을 수도 있습니다."
 
-#: fleetpings/templates/fleetpings/index.html:61
+#: fleetpings/templates/fleetpings/index.html:59
 msgid ""
 "Success! Your ping text has been copied to your clipboard. Now be a good FC "
 "and throw it in your chat so you actually get some people in fleet."
 msgstr ""
 "성공! 핑이 클립보드에 복사되었습니다. 채팅창에 핑을 붙여넣어 사람을 모아보세"
 "요."
 
@@ -547,66 +545,54 @@
 "existing translation?"
 msgstr "이 앱을 번역하거나 기존 번역을 개선하고 싶으신가요?"
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "번역가 팀에 참여하세요!"
 
-#: fleetpings/templates/fleetpings/partials/form/form.html:69
+#: fleetpings/templates/fleetpings/partials/form/form.html:68
 #, fuzzy
 #| msgid "Create Ping"
 msgid "Create ping"
 msgstr "핑 생성"
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:6
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:7
 msgid "Please think twice if you really need to ping <code>@everyone</code>."
 msgstr "정말 <code>@everyone</code> 을 사용해야 하는지 확인해 주세요."
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:10
-#, fuzzy
-#| msgid ""
-#| "\n"
-#| "                    <code>@everyone</code>\n"
-#| "                    includes also all the people in this channel who are "
-#| "offline and\n"
-#| "                    possibly asleep at the moment and might be waking up "
-#| "when their\n"
-#| "                    mobile devices ping. Or they wake up hours later to "
-#| "irrelevant\n"
-#| "                    pings by the time they open Discord.\n"
-#| "                "
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:11
 msgid ""
 "\n"
-"                <code>@everyone</code>\n"
-"                includes also all the people in this channel who are offline "
-"and\n"
-"                possibly asleep at the moment and might be waking up when "
-"their\n"
-"                mobile devices ping. Or they wake up hours later to "
+"                    <code>@everyone</code>\n"
+"                    includes also all the people in this channel who are "
+"offline and\n"
+"                    possibly asleep at the moment and might be waking up "
+"when their\n"
+"                    mobile devices ping. Or they wake up hours later to "
 "irrelevant\n"
-"                pings by the time they open Discord.\n"
-"            "
+"                    pings by the time they open Discord.\n"
+"                "
 msgstr ""
 "\n"
 "                    <code>@everyone</code>\n"
 "                    은 이 채널에 있는 오프라인인 사람을 포함한 모든 사람과\n"
 "                    자는 사람의 휴대폰을 울려 자던 사람을 깨울 수도 있습니"
 "다.\n"
 "                    또는 몇 시간 뒤 일어나서 디스코드를 열었을 때\n"
 "                    별로 중요하지 않은 내용의 핑을 볼 수도 있습니다.\n"
 "                "
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:20
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:21
 msgid ""
 "Notification spam is a real thing and might entice people to mute channels."
 msgstr ""
 "알람 스팸은 실제로 존재하며 사람들이 채널 알람을 끄게 되는 이유가 될 수 있습"
 "니다."
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:24
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:25
 msgid "<code>@here</code> usually does the trick just fine."
 msgstr "<code>@here</code> 는 사용해도 좋습니다."
 
 #: fleetpings/templates/fleetpings/partials/form/segments/fleet-type.html:3
 msgid "Please select"
 msgstr "선택해 주세요"
 
@@ -650,26 +636,26 @@
 
 #: fleetpings/templates/fleetpings/partials/ping/ping.html:22
 #, fuzzy
 #| msgid "Copy Ping Text"
 msgid "Copy ping text"
 msgstr "핑 텍스트 복사"
 
-#: fleetpings/views.py:439
+#: fleetpings/views.py:394
 msgid "Not all mandatory information available to create an SRP link."
 msgstr "SRP 링크를 생성하기 위해 필요한 필수 정보들이 부족합니다."
 
-#: fleetpings/views.py:474
+#: fleetpings/views.py:426
 msgid "Fleet operations timer has been created …"
 msgstr "함대 오퍼레이션 타이머가 생성되었습니다…"
 
-#: fleetpings/views.py:483
+#: fleetpings/views.py:435
 msgid "SRP link has been created …"
 msgstr "SRP 링크가 생성되었습니다…"
 
-#: fleetpings/views.py:500
+#: fleetpings/views.py:452
 msgid "Form invalid. Please check your input."
 msgstr "잘못된 양식. 내용을 확인해 주세요."
 
-#: fleetpings/views.py:502
+#: fleetpings/views.py:454
 msgid "No form data submitted."
 msgstr "양식 데이터가 없습니다."
```

### Comparing `aa_fleetpings-3.0.0/fleetpings/locale/ru/LC_MESSAGES/django.mo` & `aa_fleetpings-3.0.0b1/fleetpings/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/locale/ru/LC_MESSAGES/django.po` & `aa_fleetpings-3.0.0b1/fleetpings/locale/ru/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,490 +4,490 @@
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 # Nikolay <nick.postnikov@gmail.com>, 2023.
 # Max <mark25@inbox.ru>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-15 21:21+0100\n"
+"POT-Creation-Date: 2023-10-01 17:17+0200\n"
 "PO-Revision-Date: 2023-10-03 11:34+0000\n"
 "Last-Translator: Max <mark25@inbox.ru>\n"
-"Language-Team: Russian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-fleetpings/ru/>\n"
+"Language-Team: Russian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-fleetpings/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "X-Generator: Weblate 5.0.2\n"
 
-#: fleetpings/__init__.py:10 fleetpings/templates/fleetpings/base.html:6
+#: fleetpings/__init__.py:12 fleetpings/templates/fleetpings/base.html:5
 #: fleetpings/templates/fleetpings/base.html:10
 msgid "Fleet Pings"
 msgstr "Анонсы флота"
 
-#: fleetpings/admin.py:114 fleetpings/models.py:167
+#: fleetpings/admin.py:104 fleetpings/models.py:147
 msgid "Fleet comm"
 msgstr "Флит ком"
 
-#: fleetpings/admin.py:144 fleetpings/form.py:151
+#: fleetpings/admin.py:125 fleetpings/form.py:149
 msgid "Doctrine"
 msgstr "Формат"
 
-#: fleetpings/admin.py:158 fleetpings/form.py:158 fleetpings/models.py:192
+#: fleetpings/admin.py:130 fleetpings/form.py:156 fleetpings/models.py:172
 msgid "Doctrine link"
 msgstr "Ссылка на формат"
 
-#: fleetpings/admin.py:173 fleetpings/admin.py:244 fleetpings/admin.py:325
-#: fleetpings/admin.py:370 fleetpings/models.py:201 fleetpings/models.py:344
-#: fleetpings/models.py:451 fleetpings/models.py:522
+#: fleetpings/admin.py:136 fleetpings/admin.py:189 fleetpings/admin.py:243
+#: fleetpings/admin.py:288 fleetpings/models.py:181 fleetpings/models.py:308
+#: fleetpings/models.py:395 fleetpings/models.py:459
 msgid "Group restrictions"
 msgstr "Ограничения групп"
 
-#: fleetpings/admin.py:229 fleetpings/form.py:76
+#: fleetpings/admin.py:183 fleetpings/form.py:74
 msgid "Ping target"
 msgstr "Цель пинга"
 
-#: fleetpings/admin.py:289 fleetpings/form.py:93 fleetpings/models.py:485
+#: fleetpings/admin.py:225 fleetpings/form.py:91 fleetpings/models.py:422
 msgid "Fleet type"
 msgstr "Тип флота"
 
-#: fleetpings/admin.py:303 fleetpings/models.py:442
+#: fleetpings/admin.py:230 fleetpings/models.py:386
 msgid "Embed color"
 msgstr "Цвет встраивания"
 
-#: fleetpings/admin.py:359 fleetpings/models.py:500
+#: fleetpings/admin.py:277 fleetpings/models.py:437
 msgid "Discord channel"
 msgstr "Канал Discord"
 
-#: fleetpings/admin.py:364 fleetpings/models.py:513
+#: fleetpings/admin.py:282 fleetpings/models.py:450
 msgid "Webhook URL"
 msgstr "Вебхук URL"
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: fleetpings/apps.py:21
 #, python-brace-format
 msgid "Fleet Pings v{__version__}"
 msgstr "Анонс флота v{__version__}"
 
-#: fleetpings/form.py:27
+#: fleetpings/form.py:25
 msgid "Discord Markdown"
 msgstr "Разметка Discord"
 
-#: fleetpings/form.py:34
+#: fleetpings/form.py:32
 #, python-brace-format
 msgid "Hint: You can use {discord_markdown_link} to format the text."
 msgstr ""
 "Подсказка: Вы можете использовать {discord_markdown_link} для форматирования "
 "текста."
 
-#: fleetpings/form.py:78
+#: fleetpings/form.py:76
 msgid "Who do you want to ping?"
 msgstr "Кого Вы хотите пинговать?"
 
-#: fleetpings/form.py:83
+#: fleetpings/form.py:81
 msgid "Pre-Ping"
 msgstr "Предварительный пинг"
 
-#: fleetpings/form.py:84
+#: fleetpings/form.py:82
 msgid "Mark this checkbox if this should be a pre-ping."
 msgstr "Установите флажок, если это предварительный пинг."
 
-#: fleetpings/form.py:88
+#: fleetpings/form.py:86
 msgid "Ping to"
 msgstr "Пинговать в"
 
-#: fleetpings/form.py:90
+#: fleetpings/form.py:88
 msgid "Select a channel to ping automatically."
 msgstr "Выберите канал для автоматических пингов."
 
-#: fleetpings/form.py:97
+#: fleetpings/form.py:95
 msgid "FC name"
 msgstr "Ник флиткома"
 
-#: fleetpings/form.py:99
+#: fleetpings/form.py:97
 msgid "Who is the FC?"
 msgstr "Кто флитком?"
 
-#: fleetpings/form.py:103
+#: fleetpings/form.py:101
 msgid "Fleet name"
 msgstr "Название флота"
 
-#: fleetpings/form.py:107
+#: fleetpings/form.py:105
 msgid "What is the fleet name in the fleet finder in Eve?"
 msgstr "Как называется флот в поиске флотов в Eve?"
 
-#: fleetpings/form.py:113 fleetpings/models.py:305
+#: fleetpings/form.py:111 fleetpings/models.py:269
 msgid "Formup location"
 msgstr "Место сбора"
 
-#: fleetpings/form.py:120
+#: fleetpings/form.py:118
 msgid "Formup time"
 msgstr "Время сбора"
 
-#: fleetpings/form.py:124
+#: fleetpings/form.py:122
 msgid ""
 "To enable this field, either make it a pre-ping (checkbox above) or uncheck "
 "\"Formup NOW\" (checkbox below)."
 msgstr ""
 "Для активации этого поля задайте предварительный пинг (флажок выше) или "
 "отмените «СЕЙЧАС» (флажок ниже)."
 
-#: fleetpings/form.py:130
+#: fleetpings/form.py:128
 msgid "Formup timestamp"
 msgstr "Метка времени сбора"
 
-#: fleetpings/form.py:136
+#: fleetpings/form.py:134
 msgid "Formup NOW"
 msgstr "Сбор СЕЙЧАС"
 
-#: fleetpings/form.py:138
+#: fleetpings/form.py:136
 msgid ""
 "If this checkbox is active, formup time will be set to \"NOW\" and the time "
 "in the field above (if any is set) will be ignored."
 msgstr ""
 "Если флажок активен, время сбора будет задано «СЕЙЧАС» и заданное выше время "
 "(при наличии) будет проигнорировано."
 
-#: fleetpings/form.py:144 fleetpings/models.py:168
+#: fleetpings/form.py:142 fleetpings/models.py:148
 msgid "Fleet comms"
 msgstr "Вид голосовой связи"
 
-#: fleetpings/form.py:163
+#: fleetpings/form.py:161
 msgid "Webhook embed color"
 msgstr "Цвет фона анонса"
 
-#: fleetpings/form.py:169
+#: fleetpings/form.py:167
 msgid "SRP"
 msgstr "Компенс"
 
-#: fleetpings/form.py:170
+#: fleetpings/form.py:168
 msgid "Is this fleet covered by SRP?"
 msgstr "Компенс есть?"
 
-#: fleetpings/form.py:175
+#: fleetpings/form.py:173
 msgid "Create SRP link"
 msgstr "Создание SRP ссылки"
 
-#: fleetpings/form.py:177
+#: fleetpings/form.py:175
 msgid ""
 "If this checkbox is active, a SRP link specific for this fleet will be "
 "created.<br>Leave blank if unsure."
 msgstr ""
-"Если флажок активен, специальная ссылка для компенса будет создана."
-"<br>Оставьте неактивным, если не уверены."
+"Если флажок активен, специальная ссылка для компенса будет "
+"создана.<br>Оставьте неактивным, если не уверены."
 
-#: fleetpings/form.py:183
+#: fleetpings/form.py:181
 msgid "Additional information"
 msgstr "Дополнительная информация"
 
-#: fleetpings/form.py:190
+#: fleetpings/form.py:188
 msgid "Feel free to add some more information about the fleet …"
 msgstr "Разместите любую дополнительную информацию о флоте …"
 
-#: fleetpings/form.py:199
+#: fleetpings/form.py:197
 msgid "Create Optimer"
 msgstr "Создать таймер"
 
-#: fleetpings/form.py:201
+#: fleetpings/form.py:199
 msgid ""
 "If this checkbox is active, a fleet operations timer for this pre-ping will "
 "be created."
 msgstr ""
 "Если флажок активен, будет создан специальный таймер сбора для данного "
 "предварительно пинга."
 
-#: fleetpings/models.py:41
+#: fleetpings/models.py:40
 msgid "You might want to install the Discord service first …"
 msgstr "Возможно, Вам следует сначала установить сервис Discord …"
 
-#: fleetpings/models.py:49
+#: fleetpings/models.py:47
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr "Вы уверены, что Ваш Discord связан с Вашим Alliance Auth?"
 
-#: fleetpings/models.py:55
+#: fleetpings/models.py:51
 msgid "This group has not been synced to Discord yet."
 msgstr "Эта группа не была синхронизирована с Discord."
 
-#: fleetpings/models.py:117
+#: fleetpings/models.py:104
 msgid "Can access this app"
 msgstr "Имеет доступ к приложению"
 
-#: fleetpings/models.py:127
+#: fleetpings/models.py:114
 msgid "Short name to identify this comms"
 msgstr "Короткое название голосового канала"
 
-#: fleetpings/models.py:128 fleetpings/models.py:184 fleetpings/models.py:272
-#: fleetpings/models.py:434
+#: fleetpings/models.py:115 fleetpings/models.py:164 fleetpings/models.py:242
+#: fleetpings/models.py:378
 msgid "Name"
 msgstr "Название"
 
-#: fleetpings/models.py:134
+#: fleetpings/models.py:121
 msgid "In which channel is the fleet?"
 msgstr "Который из каналов назначен для флота?"
 
-#: fleetpings/models.py:135
+#: fleetpings/models.py:122
 msgid "Channel"
 msgstr "Канал"
 
-#: fleetpings/models.py:141 fleetpings/models.py:208 fleetpings/models.py:279
-#: fleetpings/models.py:351 fleetpings/models.py:458
+#: fleetpings/models.py:128 fleetpings/models.py:188 fleetpings/models.py:249
+#: fleetpings/models.py:315 fleetpings/models.py:402
 msgid "You can add notes about this configuration here if you want"
 msgstr "Здесь Вы можете добавить примечания для этой конфигурации"
 
-#: fleetpings/models.py:142 fleetpings/models.py:209 fleetpings/models.py:280
-#: fleetpings/models.py:352 fleetpings/models.py:459 fleetpings/models.py:530
+#: fleetpings/models.py:129 fleetpings/models.py:189 fleetpings/models.py:250
+#: fleetpings/models.py:316 fleetpings/models.py:403 fleetpings/models.py:467
 msgid "Notes"
 msgstr "Примечания"
 
-#: fleetpings/models.py:148
+#: fleetpings/models.py:135
 msgid "Whether this comms is enabled or not"
 msgstr "Активен или нет голосовой канал"
 
-#: fleetpings/models.py:149 fleetpings/models.py:217 fleetpings/models.py:288
-#: fleetpings/models.py:360 fleetpings/models.py:467 fleetpings/models.py:538
+#: fleetpings/models.py:136 fleetpings/models.py:197 fleetpings/models.py:258
+#: fleetpings/models.py:324 fleetpings/models.py:411 fleetpings/models.py:475
 msgid "Is enabled"
 msgstr "Разрешен"
 
-#: fleetpings/models.py:183
+#: fleetpings/models.py:163
 msgid "Short name to identify this doctrine"
 msgstr "Короткое название формата"
 
-#: fleetpings/models.py:191
+#: fleetpings/models.py:171
 msgid "A link to a doctrine page for this doctrine if you have."
 msgstr "Ссылка на страницу формата."
 
-#: fleetpings/models.py:200
+#: fleetpings/models.py:180
 msgid "Restrict this doctrine to the following groups …"
 msgstr "Предоставить доступ к формату следующим группам …"
 
-#: fleetpings/models.py:216
+#: fleetpings/models.py:196
 msgid "Whether this doctrine is enabled or not"
 msgstr "Активен или нет формат"
 
-#: fleetpings/models.py:237
+#: fleetpings/models.py:214
 msgid "Your doctrine URL is not valid."
 msgstr "URL формата некорректный."
 
-#: fleetpings/models.py:257
+#: fleetpings/models.py:227
 msgid "Fleet doctrine"
 msgstr "Формат флота"
 
-#: fleetpings/models.py:258
+#: fleetpings/models.py:228
 msgid "Fleet doctrines"
 msgstr "Форматы"
 
-#: fleetpings/models.py:271
+#: fleetpings/models.py:241
 msgid "Short name to identify this formup location"
 msgstr "Короткое название точки сбора"
 
-#: fleetpings/models.py:287 fleetpings/models.py:359
+#: fleetpings/models.py:257 fleetpings/models.py:323
 msgid "Whether this formup location is enabled or not"
 msgstr "Активна или нет точка сбора"
 
-#: fleetpings/models.py:306
+#: fleetpings/models.py:270
 msgid "Formup locations"
 msgstr "Места сбора"
 
-#: fleetpings/models.py:322
+#: fleetpings/models.py:286
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 "Имя роли Discord для пинга. (Примечание: Это должна быть синхронизированная "
 "с Discord группа Auth.)"
 
-#: fleetpings/models.py:326
+#: fleetpings/models.py:290
 msgid "Group name"
 msgstr "Имя группы"
 
-#: fleetpings/models.py:334
+#: fleetpings/models.py:298
 msgid "ID of the Discord role to ping"
 msgstr "ID роли Discord для пинга"
 
-#: fleetpings/models.py:335
+#: fleetpings/models.py:299
 msgid "Discord ID"
 msgstr "Идентификатор Discord"
 
-#: fleetpings/models.py:343 fleetpings/models.py:521
+#: fleetpings/models.py:307 fleetpings/models.py:458
 msgid "Restrict ping rights to the following groups …"
 msgstr "Ограничить право пинговать для следующих групп …"
 
-#: fleetpings/models.py:419
+#: fleetpings/models.py:363
 msgid "Discord ping target"
 msgstr "Цель пинга Discrod"
 
-#: fleetpings/models.py:420
+#: fleetpings/models.py:364
 msgid "Discord ping targets"
 msgstr "Цели пинга Discord"
 
-#: fleetpings/models.py:433
+#: fleetpings/models.py:377
 msgid "Short name to identify this fleet type"
 msgstr "Короткое название типа флота"
 
-#: fleetpings/models.py:441
+#: fleetpings/models.py:385
 msgid "Highlight color for the embed"
 msgstr "Цвет при встраивании"
 
-#: fleetpings/models.py:450
+#: fleetpings/models.py:394
 msgid "Restrict this fleet type to the following groups …"
 msgstr "Предоставить доступ к флоту следующим группам …"
 
-#: fleetpings/models.py:466
+#: fleetpings/models.py:410
 msgid "Whether this fleet type is enabled or not"
 msgstr "Активен или нет тип флота"
 
-#: fleetpings/models.py:486
+#: fleetpings/models.py:423
 msgid "Fleet types"
 msgstr "Типы флота"
 
-#: fleetpings/models.py:499
+#: fleetpings/models.py:436
 msgid "Name of the channel this webhook posts to"
 msgstr "Название канала, в который вебхук отправляет сообщения"
 
-#: fleetpings/models.py:509
+#: fleetpings/models.py:446
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
 "URL этого вебхука, например https://discord.com/api/webhooks/123456/abcdef"
 
-#: fleetpings/models.py:529
+#: fleetpings/models.py:466
 msgid "You can add notes about this webhook here if you want"
 msgstr "Здесь Вы можете добавить примечания для этого вебхука"
 
-#: fleetpings/models.py:537
+#: fleetpings/models.py:474
 msgid "Whether this webhook is active or not"
 msgstr "Активен или нет вебхук"
 
-#: fleetpings/models.py:556
+#: fleetpings/models.py:486
 msgid "Webhook"
 msgstr "Вебхук"
 
-#: fleetpings/models.py:557
+#: fleetpings/models.py:487
 msgid "Webhooks"
 msgstr "Вебхуки"
 
-#: fleetpings/models.py:576
+#: fleetpings/models.py:502
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 "Некорректный URL вебхука. Введенный URL не совпадает с известными форматами "
 "вебхуков Discord. Пожалуйста, проверьте URL."
 
-#: fleetpings/models.py:596
+#: fleetpings/models.py:522
 msgid "Use default fleet types"
 msgstr "Использовать типы флотов по умолчанию"
 
-#: fleetpings/models.py:599
+#: fleetpings/models.py:525
 msgid "Use default ping targets"
 msgstr "Использовать цель пинга по умолчанию"
 
-#: fleetpings/models.py:602
+#: fleetpings/models.py:528
 msgid "Use Doctrines from Fittings module"
 msgstr "Использовать форматы из модуля Fittings"
 
-#: fleetpings/models.py:604
+#: fleetpings/models.py:530
 msgid "Verify webhooks"
 msgstr "Проверять Вебхуки"
 
-#: fleetpings/models.py:605
+#: fleetpings/models.py:531
 msgid "Default embed color"
 msgstr "Цвет встраивания по умолчанию"
 
-#: fleetpings/models.py:611
+#: fleetpings/models.py:537
 msgid ""
 "Whether to use default fleet types. If checked, the default fleet types "
 "(Roaming, Home Defense, StratOP, and CTA) will be added to the Fleet Type "
 "dropdown."
 msgstr ""
 "Использование типов флотов по умолчанию. Если установлен, стандартные типы "
 "флотов (роум, хоумдеф, стратоп и КТА) будут добавлены в список Тип Флота."
 
-#: fleetpings/models.py:622
+#: fleetpings/models.py:548
 msgid ""
 "Whether to use default ping targets. If checked, the default ping targets "
 "(@everyone and @here) will be added to the Ping Target dropdown."
 msgstr ""
 "Использование целей пинга по умолчанию. Если установлен, стандартные цели "
 "пинга (@everyone и @here) будут добавлены в список Цель Пинга."
 
-#: fleetpings/models.py:632
+#: fleetpings/models.py:558
 msgid ""
 "Whether to use the doctrines from the Fittings modules in the doctrine "
 "dropdown. Note: The fittings module needs to be installed for this."
 msgstr ""
 "Использование форматов из модуля Fittings в списке выбора формата. "
 "Примечание: модуль Fittings должен быть установлен."
 
-#: fleetpings/models.py:642
+#: fleetpings/models.py:568
 msgid ""
 "Whether to verify webhooks URLs or not. Note: When unchecked, webhook URLs "
 "will not be verified, so the app can be used with non-Discord webhooks as "
 "well. When disabling webhook verification and using non-Discord webhooks, it "
 "is up to you to make sure your webhook understands a payload that is "
 "formatted for Discord webhooks."
 msgstr ""
 "Проверка Webhooks URL. Примечание: Если сброшен, Webhook URL не будет "
 "проверяться, таким образом приложение может быть использовано с не-Discord "
 "Webhook. При выключенной проверке для не-Discord Webhook, убедитесь, что ваш "
 "Webhook понимает данные в формате Discord."
 
-#: fleetpings/models.py:655
+#: fleetpings/models.py:581
 msgid "Default highlight color for the webhook embed."
 msgstr "Цвет подсветки по умолчанию для встраивания webhook."
 
-#: fleetpings/models.py:667
+#: fleetpings/models.py:593
 msgid "Setting"
 msgstr "Установка"
 
-#: fleetpings/models.py:668
+#: fleetpings/models.py:594
 msgid "Settings"
 msgstr "Настройки"
 
-#: fleetpings/models.py:678
+#: fleetpings/models.py:597
 msgid "Fleet Pings Settings"
 msgstr "Настройки Сбора флота"
 
 #: fleetpings/templates/fleetpings/index.html:11
 msgid "Fleet information"
 msgstr "Информация о флоте"
 
-#: fleetpings/templates/fleetpings/index.html:23
+#: fleetpings/templates/fleetpings/index.html:22
 msgid "Formatted ping text"
 msgstr "Отформатированный текст пинга"
 
-#: fleetpings/templates/fleetpings/index.html:51
+#: fleetpings/templates/fleetpings/index.html:49
 msgid ""
 "Mandatory information is missing. To create an optimer, you need to provide "
 "all of the following information:<br>» FC name<br>» Fleet name<br>» Formup "
 "location<br>» Formup time<br>» Ships / Doctrine"
 msgstr ""
 "Отсутствует необходимая информация. Для создания таймера должна быть "
 "предоставлена следующая информация:<br>» Ник флиткома<br>» Имя флота<br>» "
 "Точка сбора<br>» Время сбора<br>» Корабли / Формат"
 
-#: fleetpings/templates/fleetpings/index.html:56
+#: fleetpings/templates/fleetpings/index.html:54
 msgid ""
 "Mandatory information is missing. To create an SRP link, you need to provide "
 "all of the following information:<br>» Fleet name<br>» Ships / Doctrine"
 msgstr ""
 "Отсутствует необходимая информация. Для создания ссылки для компенса должна "
 "быть предоставлена следующая информация:<br>» Имя флота<br>» Корабли / Формат"
 
-#: fleetpings/templates/fleetpings/index.html:60
+#: fleetpings/templates/fleetpings/index.html:58
 msgid ""
 "Error! Your ping was not copied to your clipboard. Maybe your browser "
 "doesn&apos;t support this feature."
 msgstr ""
 "Ошибка! Ваш пинг не был скопирован в буфер обмена. Возможно, браузер не "
 "поддерживает данную функциональность."
 
-#: fleetpings/templates/fleetpings/index.html:61
+#: fleetpings/templates/fleetpings/index.html:59
 msgid ""
 "Success! Your ping text has been copied to your clipboard. Now be a good FC "
 "and throw it in your chat so you actually get some people in fleet."
 msgstr ""
 "Успех! Текст пинга был скопирован в буфер обмена. Скопируйте сообщение в "
 "чат, чтобы пилоты могли присоединиться."
 
@@ -499,65 +499,53 @@
 "Вы хотите помочь перевести это приложение на ваш язык или улучшить текущий "
 "перевод?"
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "Присоединяйтесь к нашей команде переводчиков!"
 
-#: fleetpings/templates/fleetpings/partials/form/form.html:69
+#: fleetpings/templates/fleetpings/partials/form/form.html:68
 msgid "Create ping"
 msgstr "Создать пинг"
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:6
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:7
 msgid "Please think twice if you really need to ping <code>@everyone</code>."
 msgstr "Подумайте дважды перед тем, как пинговать <code>@everyone</code>."
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:10
-#, fuzzy
-#| msgid ""
-#| "\n"
-#| "                    <code>@everyone</code>\n"
-#| "                    includes also all the people in this channel who are "
-#| "offline and\n"
-#| "                    possibly asleep at the moment and might be waking up "
-#| "when their\n"
-#| "                    mobile devices ping. Or they wake up hours later to "
-#| "irrelevant\n"
-#| "                    pings by the time they open Discord.\n"
-#| "                "
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:11
 msgid ""
 "\n"
-"                <code>@everyone</code>\n"
-"                includes also all the people in this channel who are offline "
-"and\n"
-"                possibly asleep at the moment and might be waking up when "
-"their\n"
-"                mobile devices ping. Or they wake up hours later to "
+"                    <code>@everyone</code>\n"
+"                    includes also all the people in this channel who are "
+"offline and\n"
+"                    possibly asleep at the moment and might be waking up "
+"when their\n"
+"                    mobile devices ping. Or they wake up hours later to "
 "irrelevant\n"
-"                pings by the time they open Discord.\n"
-"            "
+"                    pings by the time they open Discord.\n"
+"                "
 msgstr ""
 "\n"
 "                    <code>@everyone</code>\n"
 "                    обозначает всех людей в канале, включая тех кто "
 "offline,\n"
 "                    возможно сейчас спит и будет разбужен звуком\n"
 "                    мобильного устройств. Или они проснуться через несколько "
 "часов\n"
 "                    и увидят неактуальные пинги в Discord.\n"
 "                "
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:20
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:21
 msgid ""
 "Notification spam is a real thing and might entice people to mute channels."
 msgstr ""
 "Спам нотификациями это злоупотребление и может заставить людей отключить "
 "звук каналу."
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:24
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:25
 msgid "<code>@here</code> usually does the trick just fine."
 msgstr "<code>@here</code> обычно решает задачу."
 
 #: fleetpings/templates/fleetpings/partials/form/segments/fleet-type.html:3
 msgid "Please select"
 msgstr "Выберите"
 
@@ -597,26 +585,26 @@
 msgid "No ping created yet …"
 msgstr "Пингов нет …"
 
 #: fleetpings/templates/fleetpings/partials/ping/ping.html:22
 msgid "Copy ping text"
 msgstr "Копировать текст пинга"
 
-#: fleetpings/views.py:439
+#: fleetpings/views.py:394
 msgid "Not all mandatory information available to create an SRP link."
 msgstr "Не вся необходимая информация предоставлена для создания ссылки SRP."
 
-#: fleetpings/views.py:474
+#: fleetpings/views.py:426
 msgid "Fleet operations timer has been created …"
 msgstr "Таймер флота был создан …"
 
-#: fleetpings/views.py:483
+#: fleetpings/views.py:435
 msgid "SRP link has been created …"
 msgstr "SRP ссылка была создана …"
 
-#: fleetpings/views.py:500
+#: fleetpings/views.py:452
 msgid "Form invalid. Please check your input."
 msgstr "Форма некорректна. Проверьте введенные данные."
 
-#: fleetpings/views.py:502
+#: fleetpings/views.py:454
 msgid "No form data submitted."
 msgstr "Данные формы не отправлены."
```

### Comparing `aa_fleetpings-3.0.0/fleetpings/locale/uk/LC_MESSAGES/django.mo` & `aa_fleetpings-3.0.0b1/fleetpings/locale/uk/LC_MESSAGES/django.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "apps/aa-fleetpings/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.4.2\n"
+"X-Generator: Weblate 5.0.2\n"
 
 msgid ""
 "\n"
 "                    <code>@everyone</code>\n"
 "                    includes also all the people in this channel who are "
 "offline and\n"
 "                    possibly asleep at the moment and might be waking up "
@@ -84,19 +84,14 @@
 
 msgid "Group name"
 msgstr "Назва групи"
 
 msgid "Group restrictions"
 msgstr "Групові обмеження"
 
-msgid "Hint: You can use {discord_markdown_link} to format the text."
-msgstr ""
-"Підказка: Ви можете використовувати {discord_markdown_link} для форматування "
-"тексту."
-
 msgid "Home Defense"
 msgstr "Захист дому"
 
 msgid "ID of the Discord role to ping"
 msgstr "Ідентифікатор ролі Discord для пінгування"
 
 msgid ""
```

### Comparing `aa_fleetpings-3.0.0/fleetpings/locale/uk/LC_MESSAGES/django.po` & `aa_fleetpings-3.0.0b1/fleetpings/locale/uk/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,560 +1,557 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Kristof <kristof@teh.ninja>, 2023.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 # "Andrii M." <elfleg0las88@gmail.com>, 2023.
-# Madz Cooper <i.sviridjuk@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-15 21:21+0100\n"
-"PO-Revision-Date: 2024-03-02 23:10+0000\n"
-"Last-Translator: Madz Cooper <i.sviridjuk@gmail.com>\n"
-"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-fleetpings/uk/>\n"
+"POT-Creation-Date: 2023-10-01 17:17+0200\n"
+"PO-Revision-Date: 2023-10-02 09:47+0000\n"
+"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
+"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-fleetpings/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.4.2\n"
+"X-Generator: Weblate 5.0.2\n"
 
-#: fleetpings/__init__.py:10 fleetpings/templates/fleetpings/base.html:6
+#: fleetpings/__init__.py:12 fleetpings/templates/fleetpings/base.html:5
 #: fleetpings/templates/fleetpings/base.html:10
 #, fuzzy
 #| msgid "Fleet Ping Tool"
 msgid "Fleet Pings"
 msgstr "Інструмент пінгування флоту"
 
-#: fleetpings/admin.py:114 fleetpings/models.py:167
+#: fleetpings/admin.py:104 fleetpings/models.py:147
 #, fuzzy
 #| msgid "Fleet Comm"
 msgid "Fleet comm"
 msgstr "Зв'язок флоту"
 
-#: fleetpings/admin.py:144 fleetpings/form.py:151
+#: fleetpings/admin.py:125 fleetpings/form.py:149
 msgid "Doctrine"
 msgstr "Доктрина"
 
-#: fleetpings/admin.py:158 fleetpings/form.py:158 fleetpings/models.py:192
+#: fleetpings/admin.py:130 fleetpings/form.py:156 fleetpings/models.py:172
 msgid "Doctrine link"
 msgstr "Посилання на доктрину"
 
-#: fleetpings/admin.py:173 fleetpings/admin.py:244 fleetpings/admin.py:325
-#: fleetpings/admin.py:370 fleetpings/models.py:201 fleetpings/models.py:344
-#: fleetpings/models.py:451 fleetpings/models.py:522
+#: fleetpings/admin.py:136 fleetpings/admin.py:189 fleetpings/admin.py:243
+#: fleetpings/admin.py:288 fleetpings/models.py:181 fleetpings/models.py:308
+#: fleetpings/models.py:395 fleetpings/models.py:459
 msgid "Group restrictions"
 msgstr "Групові обмеження"
 
-#: fleetpings/admin.py:229 fleetpings/form.py:76
+#: fleetpings/admin.py:183 fleetpings/form.py:74
 #, fuzzy
 #| msgid "Ping Target"
 msgid "Ping target"
 msgstr "Мета пінгу"
 
-#: fleetpings/admin.py:289 fleetpings/form.py:93 fleetpings/models.py:485
+#: fleetpings/admin.py:225 fleetpings/form.py:91 fleetpings/models.py:422
 #, fuzzy
 #| msgid "Fleet Type"
 msgid "Fleet type"
 msgstr "Тип флоту"
 
-#: fleetpings/admin.py:303 fleetpings/models.py:442
+#: fleetpings/admin.py:230 fleetpings/models.py:386
 #, fuzzy
 #| msgid "Webhook Embed Color"
 msgid "Embed color"
 msgstr "Колір вставки Webhook"
 
-#: fleetpings/admin.py:359 fleetpings/models.py:500
+#: fleetpings/admin.py:277 fleetpings/models.py:437
 msgid "Discord channel"
 msgstr "Канал діскорду"
 
-#: fleetpings/admin.py:364 fleetpings/models.py:513
+#: fleetpings/admin.py:282 fleetpings/models.py:450
 msgid "Webhook URL"
 msgstr "Веб-хук URL"
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: fleetpings/apps.py:21
 #, python-brace-format
 msgid "Fleet Pings v{__version__}"
 msgstr ""
 
-#: fleetpings/form.py:27
+#: fleetpings/form.py:25
 #, fuzzy
 #| msgid "Discord Markdown"
 msgid "Discord Markdown"
 msgstr "Discord markdown"
 
-#: fleetpings/form.py:34
+#: fleetpings/form.py:32
 #, python-brace-format
 msgid "Hint: You can use {discord_markdown_link} to format the text."
 msgstr ""
-"Підказка: Ви можете використовувати {discord_markdown_link} для форматування "
-"тексту."
 
-#: fleetpings/form.py:78
+#: fleetpings/form.py:76
 msgid "Who do you want to ping?"
 msgstr "Кого ви хочете пінгувати?"
 
-#: fleetpings/form.py:83
+#: fleetpings/form.py:81
 msgid "Pre-Ping"
 msgstr "Попередній пінг"
 
-#: fleetpings/form.py:84
+#: fleetpings/form.py:82
 msgid "Mark this checkbox if this should be a pre-ping."
 msgstr "Відмітьте цей прапорець, якщо це має бути попередній пінг."
 
-#: fleetpings/form.py:88
+#: fleetpings/form.py:86
 #, fuzzy
 #| msgid "Ping To"
 msgid "Ping to"
 msgstr "Кого пінгувати"
 
-#: fleetpings/form.py:90
+#: fleetpings/form.py:88
 msgid "Select a channel to ping automatically."
 msgstr "Виберіть канал для автоматичного пінгування."
 
-#: fleetpings/form.py:97
+#: fleetpings/form.py:95
 msgid "FC name"
 msgstr ""
 
-#: fleetpings/form.py:99
+#: fleetpings/form.py:97
 msgid "Who is the FC?"
 msgstr "Хто ФК?"
 
-#: fleetpings/form.py:103
+#: fleetpings/form.py:101
 #, fuzzy
 #| msgid "Fleet Name"
 msgid "Fleet name"
 msgstr "Назва флоту"
 
-#: fleetpings/form.py:107
+#: fleetpings/form.py:105
 #, fuzzy
 #| msgid "What is the fleet name in fleet finder?"
 msgid "What is the fleet name in the fleet finder in Eve?"
 msgstr "Як називається флот у пошуку флоту?"
 
-#: fleetpings/form.py:113 fleetpings/models.py:305
+#: fleetpings/form.py:111 fleetpings/models.py:269
 #, fuzzy
 #| msgid "Formup Location"
 msgid "Formup location"
 msgstr "Місце формування"
 
-#: fleetpings/form.py:120
+#: fleetpings/form.py:118
 #, fuzzy
 #| msgid "Formup Time"
 msgid "Formup time"
 msgstr "Час формування"
 
-#: fleetpings/form.py:124
+#: fleetpings/form.py:122
 msgid ""
 "To enable this field, either make it a pre-ping (checkbox above) or uncheck "
 "\"Formup NOW\" (checkbox below)."
 msgstr ""
 "Щоб увімкнути це поле, зробіть його попереднім пінгом (прапорець вище) або "
 "зніміть прапорець «Створити ЗАРАЗ» (прапорець нижче)."
 
-#: fleetpings/form.py:130
+#: fleetpings/form.py:128
 #, fuzzy
 #| msgid "Formup Timestamp"
 msgid "Formup timestamp"
 msgstr "Мітка часу(timestamp) для формування"
 
-#: fleetpings/form.py:136
+#: fleetpings/form.py:134
 msgid "Formup NOW"
 msgstr "Формування зараз"
 
-#: fleetpings/form.py:138
+#: fleetpings/form.py:136
 msgid ""
 "If this checkbox is active, formup time will be set to \"NOW\" and the time "
 "in the field above (if any is set) will be ignored."
 msgstr ""
 "Якщо цей прапорець активний, час формування буде встановлено на «ЗАРАЗ», а "
 "час у полі вище (якщо він встановлений) буде проігноровано."
 
-#: fleetpings/form.py:144 fleetpings/models.py:168
+#: fleetpings/form.py:142 fleetpings/models.py:148
 #, fuzzy
 #| msgid "Fleet Comms"
 msgid "Fleet comms"
 msgstr "Канал зв'язку для флоту"
 
-#: fleetpings/form.py:163
+#: fleetpings/form.py:161
 #, fuzzy
 #| msgid "Webhook Embed Color"
 msgid "Webhook embed color"
 msgstr "Колір вставки Webhook"
 
-#: fleetpings/form.py:169
+#: fleetpings/form.py:167
 msgid "SRP"
 msgstr "srp"
 
-#: fleetpings/form.py:170
+#: fleetpings/form.py:168
 msgid "Is this fleet covered by SRP?"
 msgstr "Чи поширюється на цей флот дія SRP?"
 
-#: fleetpings/form.py:175
+#: fleetpings/form.py:173
 #, fuzzy
 #| msgid "Create SRP Link"
 msgid "Create SRP link"
 msgstr "Створіть SRP-посилання"
 
-#: fleetpings/form.py:177
+#: fleetpings/form.py:175
 msgid ""
 "If this checkbox is active, a SRP link specific for this fleet will be "
 "created.<br>Leave blank if unsure."
 msgstr ""
 "Якщо цей прапорець активний, буде створено SRP-посилання, специфічне для "
 "цього флоту.<br>Залишіть порожнім, якщо ви не впевнені."
 
-#: fleetpings/form.py:183
+#: fleetpings/form.py:181
 #, fuzzy
 #| msgid "Additional Information"
 msgid "Additional information"
 msgstr "Додаткова інформація"
 
-#: fleetpings/form.py:190
+#: fleetpings/form.py:188
 #, fuzzy
 #| msgid "Feel free to add some more information about the fleet…"
 msgid "Feel free to add some more information about the fleet …"
 msgstr "Не соромтеся додавати додаткову інформацію про флот…"
 
-#: fleetpings/form.py:199
+#: fleetpings/form.py:197
 msgid "Create Optimer"
 msgstr "Створити таймер операції"
 
-#: fleetpings/form.py:201
+#: fleetpings/form.py:199
 msgid ""
 "If this checkbox is active, a fleet operations timer for this pre-ping will "
 "be created."
 msgstr ""
 "Якщо цей прапорець активний, буде створено таймер операцій флоту для цього "
 "попереднього пінгу."
 
-#: fleetpings/models.py:41
+#: fleetpings/models.py:40
 msgid "You might want to install the Discord service first …"
 msgstr "Можливо, ви захочете спочатку встановити службу Discord …"
 
-#: fleetpings/models.py:49
+#: fleetpings/models.py:47
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr "Ви впевнені, що ваш Discord пов'язаний з вашим Alliance Auth?"
 
-#: fleetpings/models.py:55
+#: fleetpings/models.py:51
 msgid "This group has not been synced to Discord yet."
 msgstr "Цю групу ще не синхронізовано з Discord."
 
-#: fleetpings/models.py:117
+#: fleetpings/models.py:104
 msgid "Can access this app"
 msgstr ""
 
-#: fleetpings/models.py:127
+#: fleetpings/models.py:114
 msgid "Short name to identify this comms"
 msgstr "Коротка назва для ідентифікації цього каналу зв'язку"
 
-#: fleetpings/models.py:128 fleetpings/models.py:184 fleetpings/models.py:272
-#: fleetpings/models.py:434
+#: fleetpings/models.py:115 fleetpings/models.py:164 fleetpings/models.py:242
+#: fleetpings/models.py:378
 msgid "Name"
 msgstr "Назва"
 
-#: fleetpings/models.py:134
+#: fleetpings/models.py:121
 msgid "In which channel is the fleet?"
 msgstr ""
 
-#: fleetpings/models.py:135
+#: fleetpings/models.py:122
 msgid "Channel"
 msgstr ""
 
-#: fleetpings/models.py:141 fleetpings/models.py:208 fleetpings/models.py:279
-#: fleetpings/models.py:351 fleetpings/models.py:458
+#: fleetpings/models.py:128 fleetpings/models.py:188 fleetpings/models.py:249
+#: fleetpings/models.py:315 fleetpings/models.py:402
 msgid "You can add notes about this configuration here if you want"
 msgstr "Ви можете додати примітки про цю конфігурацію тут, якщо хочете"
 
-#: fleetpings/models.py:142 fleetpings/models.py:209 fleetpings/models.py:280
-#: fleetpings/models.py:352 fleetpings/models.py:459 fleetpings/models.py:530
+#: fleetpings/models.py:129 fleetpings/models.py:189 fleetpings/models.py:250
+#: fleetpings/models.py:316 fleetpings/models.py:403 fleetpings/models.py:467
 msgid "Notes"
 msgstr ""
 
-#: fleetpings/models.py:148
+#: fleetpings/models.py:135
 msgid "Whether this comms is enabled or not"
 msgstr "Увімкнено цей канал зв'язку чи ні"
 
-#: fleetpings/models.py:149 fleetpings/models.py:217 fleetpings/models.py:288
-#: fleetpings/models.py:360 fleetpings/models.py:467 fleetpings/models.py:538
+#: fleetpings/models.py:136 fleetpings/models.py:197 fleetpings/models.py:258
+#: fleetpings/models.py:324 fleetpings/models.py:411 fleetpings/models.py:475
 msgid "Is enabled"
 msgstr "Дозволено"
 
-#: fleetpings/models.py:183
+#: fleetpings/models.py:163
 msgid "Short name to identify this doctrine"
 msgstr "Коротка назва для ідентифікації цієї доктрини"
 
-#: fleetpings/models.py:191
+#: fleetpings/models.py:171
 msgid "A link to a doctrine page for this doctrine if you have."
 msgstr "Посилання на сторінку доктрини для цієї доктрини, якщо вона у вас є."
 
-#: fleetpings/models.py:200
+#: fleetpings/models.py:180
 #, fuzzy
 #| msgid "Restrict this doctrine to the following group(s) …"
 msgid "Restrict this doctrine to the following groups …"
 msgstr "Обмежте цю доктрину наступними групами …"
 
-#: fleetpings/models.py:216
+#: fleetpings/models.py:196
 msgid "Whether this doctrine is enabled or not"
 msgstr "Включена ця доктрина чи ні"
 
-#: fleetpings/models.py:237
+#: fleetpings/models.py:214
 msgid "Your doctrine URL is not valid."
 msgstr "Ваше посилання на доктрину невірне."
 
-#: fleetpings/models.py:257
+#: fleetpings/models.py:227
 #, fuzzy
 #| msgid "Fleet Doctrine"
 msgid "Fleet doctrine"
 msgstr "Доктрина флоту"
 
-#: fleetpings/models.py:258
+#: fleetpings/models.py:228
 #, fuzzy
 #| msgid "Fleet Doctrines"
 msgid "Fleet doctrines"
 msgstr "Доктрини флоту"
 
-#: fleetpings/models.py:271
+#: fleetpings/models.py:241
 msgid "Short name to identify this formup location"
 msgstr "Коротка назва для ідентифікації цього місця формування"
 
-#: fleetpings/models.py:287 fleetpings/models.py:359
+#: fleetpings/models.py:257 fleetpings/models.py:323
 msgid "Whether this formup location is enabled or not"
 msgstr "Чи ввімкнено це місце формування чи ні"
 
-#: fleetpings/models.py:306
+#: fleetpings/models.py:270
 #, fuzzy
 #| msgid "Formup Locations"
 msgid "Formup locations"
 msgstr "Місця формування"
 
-#: fleetpings/models.py:322
+#: fleetpings/models.py:286
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 "Ім'я ролі Discord, яку потрібно пінгувати. (Примітка: це має бути група "
 "Auth, яка синхронізована з Discord.)"
 
-#: fleetpings/models.py:326
+#: fleetpings/models.py:290
 msgid "Group name"
 msgstr "Назва групи"
 
-#: fleetpings/models.py:334
+#: fleetpings/models.py:298
 msgid "ID of the Discord role to ping"
 msgstr "Ідентифікатор ролі Discord для пінгування"
 
-#: fleetpings/models.py:335
+#: fleetpings/models.py:299
 #, fuzzy
 #| msgid "Discord Markdown"
 msgid "Discord ID"
 msgstr "Discord markdown"
 
-#: fleetpings/models.py:343 fleetpings/models.py:521
+#: fleetpings/models.py:307 fleetpings/models.py:458
 #, fuzzy
 #| msgid "Restrict ping rights to the following group(s) …"
 msgid "Restrict ping rights to the following groups …"
 msgstr "Обмежити права на пінг для наступних груп …"
 
-#: fleetpings/models.py:419
+#: fleetpings/models.py:363
 #, fuzzy
 #| msgid "Discord Ping Target"
 msgid "Discord ping target"
 msgstr "Ціль для пінгу в Discord"
 
-#: fleetpings/models.py:420
+#: fleetpings/models.py:364
 #, fuzzy
 #| msgid "Discord Ping Targets"
 msgid "Discord ping targets"
 msgstr "Цілі для пінгу в Discord"
 
-#: fleetpings/models.py:433
+#: fleetpings/models.py:377
 msgid "Short name to identify this fleet type"
 msgstr "Коротка назва для ідентифікації цього типу флоту"
 
-#: fleetpings/models.py:441
+#: fleetpings/models.py:385
 #, fuzzy
 #| msgid "Hightlight color for the embed"
 msgid "Highlight color for the embed"
 msgstr "Виділіть колір для вставки"
 
-#: fleetpings/models.py:450
+#: fleetpings/models.py:394
 #, fuzzy
 #| msgid "Restrict this fleet type to the following group(s) …"
 msgid "Restrict this fleet type to the following groups …"
 msgstr "Обмежте цей тип флоту наступними групами …"
 
-#: fleetpings/models.py:466
+#: fleetpings/models.py:410
 msgid "Whether this fleet type is enabled or not"
 msgstr "Увімкнено цей тип флоту чи ні"
 
-#: fleetpings/models.py:486
+#: fleetpings/models.py:423
 #, fuzzy
 #| msgid "Fleet Types"
 msgid "Fleet types"
 msgstr "Типи флоту"
 
-#: fleetpings/models.py:499
+#: fleetpings/models.py:436
 msgid "Name of the channel this webhook posts to"
 msgstr "Назва каналу, на який публікується цей веб-хук"
 
-#: fleetpings/models.py:509
+#: fleetpings/models.py:446
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
 "URL-адреса цього веб-хука, наприклад, https://discord.com/api/"
 "webhooks/123456/abcdef"
 
-#: fleetpings/models.py:529
+#: fleetpings/models.py:466
 msgid "You can add notes about this webhook here if you want"
 msgstr "Ви можете додати примітки про цей вебхук тут, якщо хочете"
 
-#: fleetpings/models.py:537
+#: fleetpings/models.py:474
 msgid "Whether this webhook is active or not"
 msgstr "Активний цей вебхук чи ні"
 
-#: fleetpings/models.py:556
+#: fleetpings/models.py:486
 msgid "Webhook"
 msgstr "Веб-хук"
 
-#: fleetpings/models.py:557
+#: fleetpings/models.py:487
 msgid "Webhooks"
 msgstr "Веб-хуки"
 
-#: fleetpings/models.py:576
+#: fleetpings/models.py:502
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 "Неправильна URL-адреса веб-хука. Введена вами URL-адреса веб-хука не "
 "відповідає жодному з відомих форматів веб-хуків Discord. Будь ласка, "
 "перевірте URL-адресу веб-хука."
 
-#: fleetpings/models.py:596
+#: fleetpings/models.py:522
 msgid "Use default fleet types"
 msgstr ""
 
-#: fleetpings/models.py:599
+#: fleetpings/models.py:525
 msgid "Use default ping targets"
 msgstr ""
 
-#: fleetpings/models.py:602
+#: fleetpings/models.py:528
 msgid "Use Doctrines from Fittings module"
 msgstr ""
 
-#: fleetpings/models.py:604
+#: fleetpings/models.py:530
 #, fuzzy
 #| msgid "Webhooks"
 msgid "Verify webhooks"
 msgstr "Веб-хуки"
 
-#: fleetpings/models.py:605
+#: fleetpings/models.py:531
 msgid "Default embed color"
 msgstr ""
 
-#: fleetpings/models.py:611
+#: fleetpings/models.py:537
 msgid ""
 "Whether to use default fleet types. If checked, the default fleet types "
 "(Roaming, Home Defense, StratOP, and CTA) will be added to the Fleet Type "
 "dropdown."
 msgstr ""
 
-#: fleetpings/models.py:622
+#: fleetpings/models.py:548
 msgid ""
 "Whether to use default ping targets. If checked, the default ping targets "
 "(@everyone and @here) will be added to the Ping Target dropdown."
 msgstr ""
 
-#: fleetpings/models.py:632
+#: fleetpings/models.py:558
 msgid ""
 "Whether to use the doctrines from the Fittings modules in the doctrine "
 "dropdown. Note: The fittings module needs to be installed for this."
 msgstr ""
 
-#: fleetpings/models.py:642
+#: fleetpings/models.py:568
 msgid ""
 "Whether to verify webhooks URLs or not. Note: When unchecked, webhook URLs "
 "will not be verified, so the app can be used with non-Discord webhooks as "
 "well. When disabling webhook verification and using non-Discord webhooks, it "
 "is up to you to make sure your webhook understands a payload that is "
 "formatted for Discord webhooks."
 msgstr ""
 
-#: fleetpings/models.py:655
+#: fleetpings/models.py:581
 msgid "Default highlight color for the webhook embed."
 msgstr "Виділіть колір для вставки."
 
-#: fleetpings/models.py:667
+#: fleetpings/models.py:593
 msgid "Setting"
 msgstr ""
 
-#: fleetpings/models.py:668
+#: fleetpings/models.py:594
 #, fuzzy
 #| msgid "Fleet Ping Tool"
 msgid "Settings"
 msgstr "Інструмент пінгування флоту"
 
-#: fleetpings/models.py:678
+#: fleetpings/models.py:597
 msgid "Fleet Pings Settings"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/index.html:11
 #, fuzzy
 #| msgid "Fleet Information"
 msgid "Fleet information"
 msgstr "Інформація про флот"
 
-#: fleetpings/templates/fleetpings/index.html:23
+#: fleetpings/templates/fleetpings/index.html:22
 #, fuzzy
 #| msgid "Formatted Ping Text"
 msgid "Formatted ping text"
 msgstr "Відформатований текст пінгу"
 
-#: fleetpings/templates/fleetpings/index.html:51
+#: fleetpings/templates/fleetpings/index.html:49
 #, fuzzy
 #| msgid ""
 #| "Mandatory information is missing. To create an optimer, you need to "
 #| "provide all of the following information:<br>» FC Name<br>» Fleet "
 #| "Name<br>» Formup Location<br>» Formup Time<br>» Ships / Doctrine"
 msgid ""
 "Mandatory information is missing. To create an optimer, you need to provide "
 "all of the following information:<br>» FC name<br>» Fleet name<br>» Formup "
 "location<br>» Formup time<br>» Ships / Doctrine"
 msgstr ""
 "Обов'язкова інформація відсутня. Для того щоб створити пінг флотової "
 "операції ви маєте заповнити всю інформацію нижче: <br>» Нік ФК<br>» Назва "
 "флоту<br>» Місце формування<br>» Чис формування<br>» Кораблі / Доктрина"
 
-#: fleetpings/templates/fleetpings/index.html:56
+#: fleetpings/templates/fleetpings/index.html:54
 #, fuzzy
 #| msgid ""
 #| "Mandatory information is missing. To create an SRP link, you need to "
 #| "provide all of the following information:<br>» Fleet Name<br>» Ships / "
 #| "Doctrine"
 msgid ""
 "Mandatory information is missing. To create an SRP link, you need to provide "
 "all of the following information:<br>» Fleet name<br>» Ships / Doctrine"
 msgstr ""
 "Обов'язкова інформація відсутня. Щоб створити посилання SRP, вам потрібно "
 "надати всю наступну інформацію: <br> » Назва флоту <br> » Кораблі / Доктрина"
 
-#: fleetpings/templates/fleetpings/index.html:60
+#: fleetpings/templates/fleetpings/index.html:58
 msgid ""
 "Error! Your ping was not copied to your clipboard. Maybe your browser "
 "doesn&apos;t support this feature."
 msgstr ""
 "Помилка! Ваш пінг не було скопійовано до буфера обміну. Можливо, ваш браузер "
 "не підтримує цю функцію."
 
-#: fleetpings/templates/fleetpings/index.html:61
+#: fleetpings/templates/fleetpings/index.html:59
 msgid ""
 "Success! Your ping text has been copied to your clipboard. Now be a good FC "
 "and throw it in your chat so you actually get some people in fleet."
 msgstr ""
 "Успішно! Текст вашого пінгу було скопійовано до буфера обміну. Тепер будь "
 "хорошим ФК і кинь його у свій чат, щоб дійсно отримати кілька людей у флот."
 
@@ -564,66 +561,54 @@
 "existing translation?"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/form.html:69
+#: fleetpings/templates/fleetpings/partials/form/form.html:68
 #, fuzzy
 #| msgid "Create Ping"
 msgid "Create ping"
 msgstr "Створити пінг"
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:6
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:7
 msgid "Please think twice if you really need to ping <code>@everyone</code>."
 msgstr ""
 "Будь ласка, подумайте двічі, якщо вам дійсно потрібно пінгувати "
 "<code>@everybody</code>."
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:10
-#, fuzzy
-#| msgid ""
-#| "\n"
-#| "                    <code>@everyone</code>\n"
-#| "                    includes also all the people in this channel who are "
-#| "offline and\n"
-#| "                    possibly asleep at the moment and might be waking up "
-#| "when their\n"
-#| "                    mobile devices ping. Or they wake up hours later to "
-#| "irrelevant\n"
-#| "                    pings by the time they open Discord.\n"
-#| "                "
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:11
 msgid ""
 "\n"
-"                <code>@everyone</code>\n"
-"                includes also all the people in this channel who are offline "
-"and\n"
-"                possibly asleep at the moment and might be waking up when "
-"their\n"
-"                mobile devices ping. Or they wake up hours later to "
+"                    <code>@everyone</code>\n"
+"                    includes also all the people in this channel who are "
+"offline and\n"
+"                    possibly asleep at the moment and might be waking up "
+"when their\n"
+"                    mobile devices ping. Or they wake up hours later to "
 "irrelevant\n"
-"                pings by the time they open Discord.\n"
-"            "
+"                    pings by the time they open Discord.\n"
+"                "
 msgstr ""
 "\n"
 "                    <code>@everyone</code> включає всіх людей в цьому "
 "каналі, які не в мережі, можливо сплять в цей момент, але можуть "
 "прокинутися, коли їх мобільні пристрої сповіщатимуть. Або вони прокинуться "
 "годинами пізніше до непотрібних повідомлень, коли вони відкриють Discord.\n"
 "                "
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:20
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:21
 msgid ""
 "Notification spam is a real thing and might entice people to mute channels."
 msgstr ""
 "Спам у сповіщеннях - це реальна річ, і він може спокусити людей вимкнути "
 "канали."
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:24
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:25
 msgid "<code>@here</code> usually does the trick just fine."
 msgstr "<code>@here</code> зазвичай чудово справляється з цим завданням."
 
 #: fleetpings/templates/fleetpings/partials/form/segments/fleet-type.html:3
 msgid "Please select"
 msgstr "Будь ласка, оберіть"
 
@@ -667,26 +652,26 @@
 
 #: fleetpings/templates/fleetpings/partials/ping/ping.html:22
 #, fuzzy
 #| msgid "Copy Ping Text"
 msgid "Copy ping text"
 msgstr "Скопіювати текст пінгу"
 
-#: fleetpings/views.py:439
+#: fleetpings/views.py:394
 msgid "Not all mandatory information available to create an SRP link."
 msgstr "Не вся обов'язкова інформація доступна для створення SRP-посилання."
 
-#: fleetpings/views.py:474
+#: fleetpings/views.py:426
 msgid "Fleet operations timer has been created …"
 msgstr "Створено таймер операцій флоту …"
 
-#: fleetpings/views.py:483
+#: fleetpings/views.py:435
 msgid "SRP link has been created …"
 msgstr "Створено SRP-посилання …"
 
-#: fleetpings/views.py:500
+#: fleetpings/views.py:452
 msgid "Form invalid. Please check your input."
 msgstr "Форма невірна. Будь ласка, перевірте свої дані."
 
-#: fleetpings/views.py:502
+#: fleetpings/views.py:454
 msgid "No form data submitted."
 msgstr "Не подано жодних даних."
```

### Comparing `aa_fleetpings-3.0.0/fleetpings/locale/zh_Hans/LC_MESSAGES/django.mo` & `aa_fleetpings-3.0.0b1/fleetpings/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_fleetpings-3.0.0b1/fleetpings/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -3,457 +3,457 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Faer Yili <yilifaer@gmail.com>, 2024.
 # Dehao Wu <wudehao2000@163.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-15 21:21+0100\n"
+"POT-Creation-Date: 2023-10-01 17:17+0200\n"
 "PO-Revision-Date: 2024-01-11 21:04+0000\n"
 "Last-Translator: Dehao Wu <wudehao2000@163.com>\n"
 "Language-Team: Chinese (Simplified) <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-fleetpings/zh_Hans/>\n"
 "Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "X-Generator: Weblate 5.3.1\n"
 
-#: fleetpings/__init__.py:10 fleetpings/templates/fleetpings/base.html:6
+#: fleetpings/__init__.py:12 fleetpings/templates/fleetpings/base.html:5
 #: fleetpings/templates/fleetpings/base.html:10
 msgid "Fleet Pings"
 msgstr ""
 
-#: fleetpings/admin.py:114 fleetpings/models.py:167
+#: fleetpings/admin.py:104 fleetpings/models.py:147
 msgid "Fleet comm"
 msgstr ""
 
-#: fleetpings/admin.py:144 fleetpings/form.py:151
+#: fleetpings/admin.py:125 fleetpings/form.py:149
 msgid "Doctrine"
 msgstr "舰船要求"
 
-#: fleetpings/admin.py:158 fleetpings/form.py:158 fleetpings/models.py:192
+#: fleetpings/admin.py:130 fleetpings/form.py:156 fleetpings/models.py:172
 msgid "Doctrine link"
 msgstr ""
 
-#: fleetpings/admin.py:173 fleetpings/admin.py:244 fleetpings/admin.py:325
-#: fleetpings/admin.py:370 fleetpings/models.py:201 fleetpings/models.py:344
-#: fleetpings/models.py:451 fleetpings/models.py:522
+#: fleetpings/admin.py:136 fleetpings/admin.py:189 fleetpings/admin.py:243
+#: fleetpings/admin.py:288 fleetpings/models.py:181 fleetpings/models.py:308
+#: fleetpings/models.py:395 fleetpings/models.py:459
 msgid "Group restrictions"
 msgstr ""
 
-#: fleetpings/admin.py:229 fleetpings/form.py:76
+#: fleetpings/admin.py:183 fleetpings/form.py:74
 msgid "Ping target"
 msgstr ""
 
-#: fleetpings/admin.py:289 fleetpings/form.py:93 fleetpings/models.py:485
+#: fleetpings/admin.py:225 fleetpings/form.py:91 fleetpings/models.py:422
 msgid "Fleet type"
 msgstr "舰队类型"
 
-#: fleetpings/admin.py:303 fleetpings/models.py:442
+#: fleetpings/admin.py:230 fleetpings/models.py:386
 msgid "Embed color"
 msgstr ""
 
-#: fleetpings/admin.py:359 fleetpings/models.py:500
+#: fleetpings/admin.py:277 fleetpings/models.py:437
 msgid "Discord channel"
 msgstr ""
 
-#: fleetpings/admin.py:364 fleetpings/models.py:513
+#: fleetpings/admin.py:282 fleetpings/models.py:450
 msgid "Webhook URL"
 msgstr ""
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: fleetpings/apps.py:21
 #, python-brace-format
 msgid "Fleet Pings v{__version__}"
 msgstr ""
 
-#: fleetpings/form.py:27
+#: fleetpings/form.py:25
 msgid "Discord Markdown"
 msgstr ""
 
-#: fleetpings/form.py:34
+#: fleetpings/form.py:32
 #, python-brace-format
 msgid "Hint: You can use {discord_markdown_link} to format the text."
 msgstr ""
 
-#: fleetpings/form.py:78
+#: fleetpings/form.py:76
 msgid "Who do you want to ping?"
 msgstr ""
 
-#: fleetpings/form.py:83
+#: fleetpings/form.py:81
 msgid "Pre-Ping"
 msgstr ""
 
-#: fleetpings/form.py:84
+#: fleetpings/form.py:82
 msgid "Mark this checkbox if this should be a pre-ping."
 msgstr ""
 
-#: fleetpings/form.py:88
+#: fleetpings/form.py:86
 msgid "Ping to"
 msgstr ""
 
-#: fleetpings/form.py:90
+#: fleetpings/form.py:88
 msgid "Select a channel to ping automatically."
 msgstr ""
 
-#: fleetpings/form.py:97
+#: fleetpings/form.py:95
 msgid "FC name"
 msgstr ""
 
-#: fleetpings/form.py:99
+#: fleetpings/form.py:97
 msgid "Who is the FC?"
 msgstr ""
 
-#: fleetpings/form.py:103
+#: fleetpings/form.py:101
 msgid "Fleet name"
 msgstr "舰队名字"
 
-#: fleetpings/form.py:107
+#: fleetpings/form.py:105
 msgid "What is the fleet name in the fleet finder in Eve?"
 msgstr ""
 
-#: fleetpings/form.py:113 fleetpings/models.py:305
+#: fleetpings/form.py:111 fleetpings/models.py:269
 msgid "Formup location"
 msgstr ""
 
-#: fleetpings/form.py:120
+#: fleetpings/form.py:118
 msgid "Formup time"
 msgstr ""
 
-#: fleetpings/form.py:124
+#: fleetpings/form.py:122
 msgid ""
 "To enable this field, either make it a pre-ping (checkbox above) or uncheck "
 "\"Formup NOW\" (checkbox below)."
 msgstr ""
 
-#: fleetpings/form.py:130
+#: fleetpings/form.py:128
 msgid "Formup timestamp"
 msgstr ""
 
-#: fleetpings/form.py:136
+#: fleetpings/form.py:134
 msgid "Formup NOW"
 msgstr ""
 
-#: fleetpings/form.py:138
+#: fleetpings/form.py:136
 msgid ""
 "If this checkbox is active, formup time will be set to \"NOW\" and the time "
 "in the field above (if any is set) will be ignored."
 msgstr ""
 
-#: fleetpings/form.py:144 fleetpings/models.py:168
+#: fleetpings/form.py:142 fleetpings/models.py:148
 msgid "Fleet comms"
 msgstr ""
 
-#: fleetpings/form.py:163
+#: fleetpings/form.py:161
 msgid "Webhook embed color"
 msgstr ""
 
-#: fleetpings/form.py:169
+#: fleetpings/form.py:167
 msgid "SRP"
 msgstr ""
 
-#: fleetpings/form.py:170
+#: fleetpings/form.py:168
 msgid "Is this fleet covered by SRP?"
 msgstr ""
 
-#: fleetpings/form.py:175
+#: fleetpings/form.py:173
 msgid "Create SRP link"
 msgstr "创建舰船补损链接"
 
-#: fleetpings/form.py:177
+#: fleetpings/form.py:175
 msgid ""
 "If this checkbox is active, a SRP link specific for this fleet will be "
 "created.<br>Leave blank if unsure."
 msgstr ""
 
-#: fleetpings/form.py:183
+#: fleetpings/form.py:181
 msgid "Additional information"
 msgstr "附加说明"
 
-#: fleetpings/form.py:190
+#: fleetpings/form.py:188
 msgid "Feel free to add some more information about the fleet …"
 msgstr ""
 
-#: fleetpings/form.py:199
+#: fleetpings/form.py:197
 msgid "Create Optimer"
 msgstr ""
 
-#: fleetpings/form.py:201
+#: fleetpings/form.py:199
 msgid ""
 "If this checkbox is active, a fleet operations timer for this pre-ping will "
 "be created."
 msgstr ""
 
-#: fleetpings/models.py:41
+#: fleetpings/models.py:40
 msgid "You might want to install the Discord service first …"
 msgstr ""
 
-#: fleetpings/models.py:49
+#: fleetpings/models.py:47
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
 
-#: fleetpings/models.py:55
+#: fleetpings/models.py:51
 msgid "This group has not been synced to Discord yet."
 msgstr ""
 
-#: fleetpings/models.py:117
+#: fleetpings/models.py:104
 msgid "Can access this app"
 msgstr "允许访问此软件"
 
-#: fleetpings/models.py:127
+#: fleetpings/models.py:114
 msgid "Short name to identify this comms"
 msgstr ""
 
-#: fleetpings/models.py:128 fleetpings/models.py:184 fleetpings/models.py:272
-#: fleetpings/models.py:434
+#: fleetpings/models.py:115 fleetpings/models.py:164 fleetpings/models.py:242
+#: fleetpings/models.py:378
 msgid "Name"
 msgstr "名字"
 
-#: fleetpings/models.py:134
+#: fleetpings/models.py:121
 msgid "In which channel is the fleet?"
 msgstr ""
 
-#: fleetpings/models.py:135
+#: fleetpings/models.py:122
 msgid "Channel"
 msgstr ""
 
-#: fleetpings/models.py:141 fleetpings/models.py:208 fleetpings/models.py:279
-#: fleetpings/models.py:351 fleetpings/models.py:458
+#: fleetpings/models.py:128 fleetpings/models.py:188 fleetpings/models.py:249
+#: fleetpings/models.py:315 fleetpings/models.py:402
 msgid "You can add notes about this configuration here if you want"
 msgstr ""
 
-#: fleetpings/models.py:142 fleetpings/models.py:209 fleetpings/models.py:280
-#: fleetpings/models.py:352 fleetpings/models.py:459 fleetpings/models.py:530
+#: fleetpings/models.py:129 fleetpings/models.py:189 fleetpings/models.py:250
+#: fleetpings/models.py:316 fleetpings/models.py:403 fleetpings/models.py:467
 msgid "Notes"
 msgstr ""
 
-#: fleetpings/models.py:148
+#: fleetpings/models.py:135
 msgid "Whether this comms is enabled or not"
 msgstr ""
 
-#: fleetpings/models.py:149 fleetpings/models.py:217 fleetpings/models.py:288
-#: fleetpings/models.py:360 fleetpings/models.py:467 fleetpings/models.py:538
+#: fleetpings/models.py:136 fleetpings/models.py:197 fleetpings/models.py:258
+#: fleetpings/models.py:324 fleetpings/models.py:411 fleetpings/models.py:475
 msgid "Is enabled"
 msgstr "已启用"
 
-#: fleetpings/models.py:183
+#: fleetpings/models.py:163
 msgid "Short name to identify this doctrine"
 msgstr ""
 
-#: fleetpings/models.py:191
+#: fleetpings/models.py:171
 msgid "A link to a doctrine page for this doctrine if you have."
 msgstr ""
 
-#: fleetpings/models.py:200
+#: fleetpings/models.py:180
 msgid "Restrict this doctrine to the following groups …"
 msgstr ""
 
-#: fleetpings/models.py:216
+#: fleetpings/models.py:196
 msgid "Whether this doctrine is enabled or not"
 msgstr ""
 
-#: fleetpings/models.py:237
+#: fleetpings/models.py:214
 msgid "Your doctrine URL is not valid."
 msgstr ""
 
-#: fleetpings/models.py:257
+#: fleetpings/models.py:227
 msgid "Fleet doctrine"
 msgstr ""
 
-#: fleetpings/models.py:258
+#: fleetpings/models.py:228
 msgid "Fleet doctrines"
 msgstr ""
 
-#: fleetpings/models.py:271
+#: fleetpings/models.py:241
 msgid "Short name to identify this formup location"
 msgstr ""
 
-#: fleetpings/models.py:287 fleetpings/models.py:359
+#: fleetpings/models.py:257 fleetpings/models.py:323
 msgid "Whether this formup location is enabled or not"
 msgstr ""
 
-#: fleetpings/models.py:306
+#: fleetpings/models.py:270
 msgid "Formup locations"
 msgstr ""
 
-#: fleetpings/models.py:322
+#: fleetpings/models.py:286
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 
-#: fleetpings/models.py:326
+#: fleetpings/models.py:290
 msgid "Group name"
 msgstr ""
 
-#: fleetpings/models.py:334
+#: fleetpings/models.py:298
 msgid "ID of the Discord role to ping"
 msgstr ""
 
-#: fleetpings/models.py:335
+#: fleetpings/models.py:299
 msgid "Discord ID"
 msgstr ""
 
-#: fleetpings/models.py:343 fleetpings/models.py:521
+#: fleetpings/models.py:307 fleetpings/models.py:458
 msgid "Restrict ping rights to the following groups …"
 msgstr ""
 
-#: fleetpings/models.py:419
+#: fleetpings/models.py:363
 msgid "Discord ping target"
 msgstr ""
 
-#: fleetpings/models.py:420
+#: fleetpings/models.py:364
 msgid "Discord ping targets"
 msgstr ""
 
-#: fleetpings/models.py:433
+#: fleetpings/models.py:377
 msgid "Short name to identify this fleet type"
 msgstr ""
 
-#: fleetpings/models.py:441
+#: fleetpings/models.py:385
 msgid "Highlight color for the embed"
 msgstr ""
 
-#: fleetpings/models.py:450
+#: fleetpings/models.py:394
 msgid "Restrict this fleet type to the following groups …"
 msgstr ""
 
-#: fleetpings/models.py:466
+#: fleetpings/models.py:410
 msgid "Whether this fleet type is enabled or not"
 msgstr ""
 
-#: fleetpings/models.py:486
+#: fleetpings/models.py:423
 msgid "Fleet types"
 msgstr "舰队类型"
 
-#: fleetpings/models.py:499
+#: fleetpings/models.py:436
 msgid "Name of the channel this webhook posts to"
 msgstr ""
 
-#: fleetpings/models.py:509
+#: fleetpings/models.py:446
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
 
-#: fleetpings/models.py:529
+#: fleetpings/models.py:466
 msgid "You can add notes about this webhook here if you want"
 msgstr ""
 
-#: fleetpings/models.py:537
+#: fleetpings/models.py:474
 msgid "Whether this webhook is active or not"
 msgstr ""
 
-#: fleetpings/models.py:556
+#: fleetpings/models.py:486
 msgid "Webhook"
 msgstr ""
 
-#: fleetpings/models.py:557
+#: fleetpings/models.py:487
 msgid "Webhooks"
 msgstr ""
 
-#: fleetpings/models.py:576
+#: fleetpings/models.py:502
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 
-#: fleetpings/models.py:596
+#: fleetpings/models.py:522
 msgid "Use default fleet types"
 msgstr ""
 
-#: fleetpings/models.py:599
+#: fleetpings/models.py:525
 msgid "Use default ping targets"
 msgstr ""
 
-#: fleetpings/models.py:602
+#: fleetpings/models.py:528
 msgid "Use Doctrines from Fittings module"
 msgstr ""
 
-#: fleetpings/models.py:604
+#: fleetpings/models.py:530
 msgid "Verify webhooks"
 msgstr ""
 
-#: fleetpings/models.py:605
+#: fleetpings/models.py:531
 msgid "Default embed color"
 msgstr ""
 
-#: fleetpings/models.py:611
+#: fleetpings/models.py:537
 msgid ""
 "Whether to use default fleet types. If checked, the default fleet types "
 "(Roaming, Home Defense, StratOP, and CTA) will be added to the Fleet Type "
 "dropdown."
 msgstr ""
 
-#: fleetpings/models.py:622
+#: fleetpings/models.py:548
 msgid ""
 "Whether to use default ping targets. If checked, the default ping targets "
 "(@everyone and @here) will be added to the Ping Target dropdown."
 msgstr ""
 
-#: fleetpings/models.py:632
+#: fleetpings/models.py:558
 msgid ""
 "Whether to use the doctrines from the Fittings modules in the doctrine "
 "dropdown. Note: The fittings module needs to be installed for this."
 msgstr ""
 
-#: fleetpings/models.py:642
+#: fleetpings/models.py:568
 msgid ""
 "Whether to verify webhooks URLs or not. Note: When unchecked, webhook URLs "
 "will not be verified, so the app can be used with non-Discord webhooks as "
 "well. When disabling webhook verification and using non-Discord webhooks, it "
 "is up to you to make sure your webhook understands a payload that is "
 "formatted for Discord webhooks."
 msgstr ""
 
-#: fleetpings/models.py:655
+#: fleetpings/models.py:581
 msgid "Default highlight color for the webhook embed."
 msgstr ""
 
-#: fleetpings/models.py:667
+#: fleetpings/models.py:593
 msgid "Setting"
 msgstr "设置"
 
-#: fleetpings/models.py:668
+#: fleetpings/models.py:594
 msgid "Settings"
 msgstr "设置"
 
-#: fleetpings/models.py:678
+#: fleetpings/models.py:597
 msgid "Fleet Pings Settings"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/index.html:11
 msgid "Fleet information"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/index.html:23
+#: fleetpings/templates/fleetpings/index.html:22
 msgid "Formatted ping text"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/index.html:51
+#: fleetpings/templates/fleetpings/index.html:49
 msgid ""
 "Mandatory information is missing. To create an optimer, you need to provide "
 "all of the following information:<br>» FC name<br>» Fleet name<br>» Formup "
 "location<br>» Formup time<br>» Ships / Doctrine"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/index.html:56
+#: fleetpings/templates/fleetpings/index.html:54
 msgid ""
 "Mandatory information is missing. To create an SRP link, you need to provide "
 "all of the following information:<br>» Fleet name<br>» Ships / Doctrine"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/index.html:60
+#: fleetpings/templates/fleetpings/index.html:58
 msgid ""
 "Error! Your ping was not copied to your clipboard. Maybe your browser "
 "doesn&apos;t support this feature."
 msgstr ""
 
-#: fleetpings/templates/fleetpings/index.html:61
+#: fleetpings/templates/fleetpings/index.html:59
 msgid ""
 "Success! Your ping text has been copied to your clipboard. Now be a good FC "
 "and throw it in your chat so you actually get some people in fleet."
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:5
 msgid ""
@@ -461,42 +461,42 @@
 "existing translation?"
 msgstr "您想帮助将此应用程序翻译成您的母语或改进现有的翻译吗?"
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "加入我们的翻译团队吧！"
 
-#: fleetpings/templates/fleetpings/partials/form/form.html:69
+#: fleetpings/templates/fleetpings/partials/form/form.html:68
 msgid "Create ping"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:6
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:7
 msgid "Please think twice if you really need to ping <code>@everyone</code>."
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:10
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:11
 msgid ""
 "\n"
-"                <code>@everyone</code>\n"
-"                includes also all the people in this channel who are offline "
-"and\n"
-"                possibly asleep at the moment and might be waking up when "
-"their\n"
-"                mobile devices ping. Or they wake up hours later to "
+"                    <code>@everyone</code>\n"
+"                    includes also all the people in this channel who are "
+"offline and\n"
+"                    possibly asleep at the moment and might be waking up "
+"when their\n"
+"                    mobile devices ping. Or they wake up hours later to "
 "irrelevant\n"
-"                pings by the time they open Discord.\n"
-"            "
+"                    pings by the time they open Discord.\n"
+"                "
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:20
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:21
 msgid ""
 "Notification spam is a real thing and might entice people to mute channels."
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:24
+#: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:25
 msgid "<code>@here</code> usually does the trick just fine."
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/form/segments/fleet-type.html:3
 msgid "Please select"
 msgstr ""
 
@@ -536,26 +536,26 @@
 msgid "No ping created yet …"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/ping/ping.html:22
 msgid "Copy ping text"
 msgstr ""
 
-#: fleetpings/views.py:439
+#: fleetpings/views.py:394
 msgid "Not all mandatory information available to create an SRP link."
 msgstr ""
 
-#: fleetpings/views.py:474
+#: fleetpings/views.py:426
 msgid "Fleet operations timer has been created …"
 msgstr ""
 
-#: fleetpings/views.py:483
+#: fleetpings/views.py:435
 msgid "SRP link has been created …"
 msgstr ""
 
-#: fleetpings/views.py:500
+#: fleetpings/views.py:452
 msgid "Form invalid. Please check your input."
 msgstr ""
 
-#: fleetpings/views.py:502
+#: fleetpings/views.py:454
 msgid "No form data submitted."
 msgstr ""
```

### Comparing `aa_fleetpings-3.0.0/fleetpings/migrations/0001_initial.py` & `aa_fleetpings-3.0.0b1/fleetpings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/migrations/0002_webhook_is_embed_description_change.py` & `aa_fleetpings-3.0.0b1/fleetpings/migrations/0002_webhook_is_embed_description_change.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/migrations/0003_fleetdoctrine_link.py` & `aa_fleetpings-3.0.0b1/fleetpings/migrations/0003_fleetdoctrine_link.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/migrations/0004_auto_20200915_1617.py` & `aa_fleetpings-3.0.0b1/fleetpings/migrations/0004_auto_20200915_1617.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/migrations/0005_fleettype_restricted_to_group.py` & `aa_fleetpings-3.0.0b1/fleetpings/migrations/0005_fleettype_restricted_to_group.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/migrations/0006_fleetdoctrine_restricted_to_group.py` & `aa_fleetpings-3.0.0b1/fleetpings/migrations/0006_fleetdoctrine_restricted_to_group.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/migrations/0007_mysql8_default_value_fixes_20201003_1232.py` & `aa_fleetpings-3.0.0b1/fleetpings/migrations/0007_mysql8_default_value_fixes_20201003_1232.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/migrations/0008_auto_20210114_1733.py` & `aa_fleetpings-3.0.0b1/fleetpings/migrations/0008_auto_20210114_1733.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/migrations/0009_remove_webhook_is_embedded_remove_webhook_type_and_more.py` & `aa_fleetpings-3.0.0b1/fleetpings/migrations/0009_remove_webhook_is_embedded_remove_webhook_type_and_more.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/migrations/0010_use_ellipsis_character_in_strings.py` & `aa_fleetpings-3.0.0b1/fleetpings/migrations/0010_use_ellipsis_character_in_strings.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/migrations/0011_settings_and_verbose_names.py` & `aa_fleetpings-3.0.0b1/fleetpings/migrations/0011_settings_and_verbose_names.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/migrations/0012_migrate_app_settings_from_local_py_to_database.py` & `aa_fleetpings-3.0.0b1/fleetpings/migrations/0012_migrate_app_settings_from_local_py_to_database.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/migrations/0013_fleetcomm_channel.py` & `aa_fleetpings-3.0.0b1/fleetpings/migrations/0013_fleetcomm_channel.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/migrations/0014_update_models.py` & `aa_fleetpings-3.0.0b1/fleetpings/migrations/0014_update_models.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/migrations/0015_alter_discordpingtarget_options_and_more.py` & `aa_fleetpings-3.0.0b1/fleetpings/migrations/0015_alter_discordpingtarget_options_and_more.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/static/fleetpings/js/fleetpings.js` & `aa_fleetpings-3.0.0b1/fleetpings/static/fleetpings/js/fleetpings.js`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/static/fleetpings/js/fleetpings.min.js` & `aa_fleetpings-3.0.0b1/fleetpings/static/fleetpings/js/fleetpings.min.js`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/static/fleetpings/js/fleetpings.min.js.map` & `aa_fleetpings-3.0.0b1/fleetpings/static/fleetpings/js/fleetpings.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/static/fleetpings/libs/flexdatalist/2.3.0/LICENSE` & `aa_fleetpings-3.0.0b1/fleetpings/static/fleetpings/libs/flexdatalist/2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/static/fleetpings/libs/flexdatalist/2.3.0/README.md` & `aa_fleetpings-3.0.0b1/fleetpings/static/fleetpings/libs/flexdatalist/2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/static/fleetpings/libs/flexdatalist/2.3.0/jquery.flexdatalist.css` & `aa_fleetpings-3.0.0b1/fleetpings/static/fleetpings/libs/flexdatalist/2.3.0/jquery.flexdatalist.css`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/static/fleetpings/libs/flexdatalist/2.3.0/jquery.flexdatalist.js` & `aa_fleetpings-3.0.0b1/fleetpings/static/fleetpings/libs/flexdatalist/2.3.0/jquery.flexdatalist.js`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/static/fleetpings/libs/flexdatalist/2.3.0/jquery.flexdatalist.min.css` & `aa_fleetpings-3.0.0b1/fleetpings/static/fleetpings/libs/flexdatalist/2.3.0/jquery.flexdatalist.min.css`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/static/fleetpings/libs/flexdatalist/2.3.0/jquery.flexdatalist.min.js` & `aa_fleetpings-3.0.0b1/fleetpings/static/fleetpings/libs/flexdatalist/2.3.0/jquery.flexdatalist.min.js`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/static/fleetpings/libs/flexdatalist/2.3.0/jquery.flexdatalist.min.js.map` & `aa_fleetpings-3.0.0b1/fleetpings/static/fleetpings/libs/flexdatalist/2.3.0/jquery.flexdatalist.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/base.html` & `aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/base.html`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/index.html` & `aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/index.html`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/partials/form/form.html` & `aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/partials/form/form.html`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html` & `aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/partials/form/segments/fleet-doctrine.html` & `aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/partials/form/segments/fleet-doctrine.html`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/partials/form/segments/fleet-type.html` & `aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/partials/form/segments/fleet-type.html`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/partials/form/segments/ping-targets.html` & `aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/partials/form/segments/ping-targets.html`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/partials/ping/copy-paste-text.html` & `aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/partials/ping/copy-paste-text.html`

 * *Files 5% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             {#Check if aa-timezones is available#}
             {% if timezones_installed %}
                 ([Time Zone Conversion]({{ SITE_URL }}{% url "timezones:index" formup_time.timestamp %}))
             {% endif %}
 
             {#Add local time#}
             <br>
-            **Formup (Local Time):** &lt;t:{{ formup_time.timestamp }}:F&gt; (&lt;t:{{ formup_time.timestamp }}:R&gt;)
+            **Formup (Local Time):** &lt;t:{{ formup_time.timestamp }}:F&gt;
         {% endif %}
     {% endif %}
 
     {#Check if fleet comms is available#}
     {% if fleet_comms %}
         <br>
         **Comms:** {{ fleet_comms }}
```

### Comparing `aa_fleetpings-3.0.0/fleetpings/templates/fleetpings/partials/ping/ping.html` & `aa_fleetpings-3.0.0b1/fleetpings/templates/fleetpings/partials/ping/ping.html`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/templatetags/fleetpings.py` & `aa_fleetpings-3.0.0b1/fleetpings/templatetags/fleetpings.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/tests/test_access.py` & `aa_fleetpings-3.0.0b1/fleetpings/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/tests/test_ajax_calls.py` & `aa_fleetpings-3.0.0b1/fleetpings/tests/test_ajax_calls.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/tests/test_auth_hooks.py` & `aa_fleetpings-3.0.0b1/fleetpings/tests/test_auth_hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             character_id=1002,
             character_name="Bruce Wayne",
             permissions=["fleetpings.basic_access"],
         )
 
         cls.html_menu = f"""
             <li class="d-flex flex-wrap m-2 p-2 pt-0 pb-0 mt-0 mb-0 me-0 pe-0">
-                <i class="nav-link fa-regular fa-bell fa-fw align-self-center me-3 "></i>
+                <i class="nav-link far fa-bell fa-fw align-self-center me-3 "></i>
                 <a class="nav-link flex-fill align-self-center me-auto" href="{reverse('fleetpings:index')}">
                     Fleet Pings
                 </a>
             </li>
         """
 
     def test_render_hook_success(self):
```

### Comparing `aa_fleetpings-3.0.0/fleetpings/tests/test_helper_eve_images.py` & `aa_fleetpings-3.0.0b1/fleetpings/tests/test_helper_eve_images.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/tests/test_installed_modules.py` & `aa_fleetpings-3.0.0b1/fleetpings/tests/test_installed_modules.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/tests/test_model_discprdpingtarget.py` & `aa_fleetpings-3.0.0b1/fleetpings/tests/test_model_discprdpingtarget.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/tests/test_model_fleetcomm.py` & `aa_fleetpings-3.0.0b1/fleetpings/tests/test_model_fleetcomm.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/tests/test_model_fleetdoctrine.py` & `aa_fleetpings-3.0.0b1/fleetpings/tests/test_model_fleetdoctrine.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/tests/test_model_fleettype.py` & `aa_fleetpings-3.0.0b1/fleetpings/tests/test_model_fleettype.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/tests/test_model_formuplocation.py` & `aa_fleetpings-3.0.0b1/fleetpings/tests/test_model_formuplocation.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/tests/test_model_setting.py` & `aa_fleetpings-3.0.0b1/fleetpings/tests/test_model_setting.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/tests/test_model_webhook.py` & `aa_fleetpings-3.0.0b1/fleetpings/tests/test_model_webhook.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/tests/test_templatetags.py` & `aa_fleetpings-3.0.0b1/fleetpings/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/fleetpings/tests/utils.py` & `aa_fleetpings-3.0.0b1/fleetpings/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/LICENSE` & `aa_fleetpings-3.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.0/README.md` & `aa_fleetpings-3.0.0b1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -47,21 +47,19 @@
 
 ______________________________________________________________________
 
 ## Installation<a name="installation"></a>
 
 > \[!NOTE\]
 >
-> **AA Fleet Pings >= 3.0.0 needs at least Alliance Auth v4.0.0!**
+> **AA Fleet Pings needs at least Alliance Auth v4.0.0!**
 >
 > Please make sure to update your Alliance Auth instance _before_ you install this
 > module or update to the latest version, otherwise an update to Alliance Auth will
 > be pulled in unsupervised.
->
-> The last version of AA Fleet Pings that supports Alliance Auth v3 is `2.26.3`.
 
 This app is a plugin for Alliance Auth. If you don't have Alliance Auth running already,
 please install it first before proceeding. (See the official [AA installation guide]
 for details)
 
 > \[!NOTE\]
 >
```

### Comparing `aa_fleetpings-3.0.0/pyproject.toml` & `aa_fleetpings-3.0.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 dynamic = [
     "version",
 ]
 dependencies = [
-    "allianceauth<5.0.0,>=4",
+    "allianceauth>=4.0.0b1",
     "allianceauth-app-utils>=1.13",
     "dhooks-lite>=0.6.1",
 ]
 [project.optional-dependencies]
 tests-allianceauth-latest = [
     "aa-srp>=1.21",
     "aa-timezones",
```

### Comparing `aa_fleetpings-3.0.0/PKG-INFO` & `aa_fleetpings-3.0.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: aa-fleetpings
-Version: 3.0.0
+Version: 3.0.0b1
 Summary: Fleet Ping Tool for Alliance Auth supporting pings via webhooks to Discord.
 Project-URL: Changelog, https://github.com/ppfeufer/aa-fleetpings/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/ppfeufer/aa-fleetpings/blob/master/README.md
 Project-URL: Donations, https://ko-fi.com/ppfeufer
 Project-URL: Homepage, https://github.com/ppfeufer/aa-fleetpings
 Project-URL: Source, https://github.com/ppfeufer/aa-fleetpings.git
 Project-URL: Tracker, https://github.com/ppfeufer/aa-fleetpings/issues
@@ -698,15 +698,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Requires-Dist: allianceauth-app-utils>=1.13
-Requires-Dist: allianceauth<5.0.0,>=4
+Requires-Dist: allianceauth>=4.0.0b1
 Requires-Dist: dhooks-lite>=0.6.1
 Provides-Extra: tests-allianceauth-latest
 Requires-Dist: aa-srp>=1.21; extra == 'tests-allianceauth-latest'
 Requires-Dist: aa-timezones; extra == 'tests-allianceauth-latest'
 Requires-Dist: coverage; extra == 'tests-allianceauth-latest'
 Requires-Dist: django-eveuniverse; extra == 'tests-allianceauth-latest'
 Requires-Dist: django-webtest; extra == 'tests-allianceauth-latest'
@@ -763,21 +763,19 @@
 
 ______________________________________________________________________
 
 ## Installation<a name="installation"></a>
 
 > \[!NOTE\]
 >
-> **AA Fleet Pings >= 3.0.0 needs at least Alliance Auth v4.0.0!**
+> **AA Fleet Pings needs at least Alliance Auth v4.0.0!**
 >
 > Please make sure to update your Alliance Auth instance _before_ you install this
 > module or update to the latest version, otherwise an update to Alliance Auth will
 > be pulled in unsupervised.
->
-> The last version of AA Fleet Pings that supports Alliance Auth v3 is `2.26.3`.
 
 This app is a plugin for Alliance Auth. If you don't have Alliance Auth running already,
 please install it first before proceeding. (See the official [AA installation guide]
 for details)
 
 > \[!NOTE\]
 >
```

