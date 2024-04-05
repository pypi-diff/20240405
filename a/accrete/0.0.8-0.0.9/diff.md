# Comparing `tmp/accrete-0.0.8.tar.gz` & `tmp/accrete-0.0.9.tar.gz`

## Comparing `accrete-0.0.8.tar` & `accrete-0.0.9.tar`

### file list

```diff
@@ -1,109 +1,110 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/__init__.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/admin.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/apps.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/decorators.py
--rw-r--r--   0        0        0    11137 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/forms.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/middleware.py
--rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/models.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/queries.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/shortcuts.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/tenant.py
--rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/tests.py
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/sequence/__init__.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/sequence/admin.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/sequence/apps.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/sequence/forms.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/sequence/models.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/sequence/queries.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/sequence/tests.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/sequence/views.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/sequence/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/sequence/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/system_mail/__init__.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/system_mail/admin.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/system_mail/apps.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/system_mail/forms.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/system_mail/models.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/system_mail/tasks.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/system_mail/tests.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/system_mail/views.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/system_mail/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/system_mail/migrations/__init__.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/admin.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/apps.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/config.py
--rw-r--r--   0        0        0    11897 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/filter.py
--rw-r--r--   0        0        0    13835 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/helper.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/tests.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/urls.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/migrations/__init__.py
--rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/static/css/accrete.css
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/static/css/icons.css
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/static/icons/Logo.svg
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/static/icons/accrete.svg
--rw-r--r--   0        0        0    19186 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/static/js/filter.js
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/static/js/list.js
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/static/js/navbar.js
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/static/js/utils.js
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/templates/django/forms/widgets/attrs.html
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/templates/django/forms/widgets/email.html
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/templates/django/forms/widgets/file.html
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/templates/django/forms/widgets/input.html
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/templates/django/forms/widgets/select.html
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/templates/django/forms/widgets/text.html
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/templates/django/forms/widgets/textarea.html
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/templates/ui/detail.html
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/templates/ui/form.html
--rw-r--r--   0        0        0     6954 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/templates/ui/layout.html
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/templates/ui/list.html
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/templates/ui/table.html
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/templates/ui/partials/actions.html
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/templates/ui/partials/filter.html
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/templates/ui/partials/form_errors.html
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/templates/ui/partials/form_modal.html
--rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/templates/ui/partials/header.html
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/templates/ui/partials/onchange_form.html
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/templates/ui/partials/pagination_detail.html
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/templates/ui/partials/pagination_list.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/templatetags/__init__.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/ui/templatetags/accrete_ui.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/user/__init__.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/user/admin.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/user/apps.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/user/middleware.py
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/user/models.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/user/tests.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/user/urls.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/user/views.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/user/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/user/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/user/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/user/migrations/__init__.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/user/templates/user/login.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/user_registration/__init__.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/user_registration/admin.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/user_registration/apps.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/user_registration/config.py
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/user_registration/forms.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/user_registration/models.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/user_registration/tests.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/user_registration/urls.py
--rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/user_registration/views.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/user_registration/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/user_registration/migrations/__init__.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/user_registration/templates/user_registration/registration.html
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/contrib/user_registration/templates/user_registration/mail_templates/confirmation_mail.html
--rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/migrations/0001_initial.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/migrations/0002_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/utils/__init__.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 accrete-0.0.8/accrete/utils/dates.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 accrete-0.0.8/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 accrete-0.0.8/LICENSE
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 accrete-0.0.8/README.md
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 accrete-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 accrete-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/__init__.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/admin.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/apps.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/config.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/decorators.py
+-rw-r--r--   0        0        0    11137 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/forms.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/middleware.py
+-rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/models.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/queries.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/shortcuts.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/tenant.py
+-rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/tests.py
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/sequence/__init__.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/sequence/admin.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/sequence/apps.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/sequence/forms.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/sequence/models.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/sequence/queries.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/sequence/tests.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/sequence/views.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/sequence/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/sequence/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/system_mail/__init__.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/system_mail/admin.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/system_mail/apps.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/system_mail/forms.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/system_mail/models.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/system_mail/tasks.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/system_mail/tests.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/system_mail/views.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/system_mail/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/system_mail/migrations/__init__.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/admin.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/apps.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/config.py
+-rw-r--r--   0        0        0    11897 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/filter.py
+-rw-r--r--   0        0        0    13274 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/helper.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/tests.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/urls.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/migrations/__init__.py
+-rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/static/css/accrete.css
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/static/css/icons.css
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/static/icons/Logo.svg
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/static/icons/accrete.svg
+-rw-r--r--   0        0        0    19186 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/static/js/filter.js
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/static/js/list.js
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/static/js/navbar.js
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/static/js/utils.js
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/templates/django/forms/widgets/attrs.html
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/templates/django/forms/widgets/email.html
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/templates/django/forms/widgets/file.html
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/templates/django/forms/widgets/input.html
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/templates/django/forms/widgets/select.html
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/templates/django/forms/widgets/text.html
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/templates/django/forms/widgets/textarea.html
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/templates/ui/detail.html
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/templates/ui/form.html
+-rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/templates/ui/layout.html
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/templates/ui/list.html
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/templates/ui/table.html
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/templates/ui/partials/actions.html
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/templates/ui/partials/filter.html
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/templates/ui/partials/form_errors.html
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/templates/ui/partials/form_modal.html
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/templates/ui/partials/header.html
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/templates/ui/partials/onchange_form.html
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/templates/ui/partials/pagination_detail.html
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/templates/ui/partials/pagination_list.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/templatetags/__init__.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/ui/templatetags/accrete_ui.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/user/__init__.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/user/admin.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/user/apps.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/user/middleware.py
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/user/models.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/user/tests.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/user/urls.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/user/views.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/user/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/user/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/user/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/user/migrations/__init__.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/user/templates/user/login.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/user_registration/__init__.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/user_registration/admin.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/user_registration/apps.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/user_registration/config.py
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/user_registration/forms.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/user_registration/models.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/user_registration/tests.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/user_registration/urls.py
+-rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/user_registration/views.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/user_registration/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/user_registration/migrations/__init__.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/user_registration/templates/user_registration/registration.html
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/contrib/user_registration/templates/user_registration/mail_templates/confirmation_mail.html
+-rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/migrations/0002_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/utils/__init__.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 accrete-0.0.9/accrete/utils/dates.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 accrete-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 accrete-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 accrete-0.0.9/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 accrete-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 accrete-0.0.9/PKG-INFO
```

### Comparing `accrete-0.0.8/accrete/admin.py` & `accrete-0.0.9/accrete/admin.py`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/forms.py` & `accrete-0.0.9/accrete/forms.py`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/middleware.py` & `accrete-0.0.9/accrete/middleware.py`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/models.py` & `accrete-0.0.9/accrete/models.py`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/tenant.py` & `accrete-0.0.9/accrete/tenant.py`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/tests.py` & `accrete-0.0.9/accrete/tests.py`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/views.py` & `accrete-0.0.9/accrete/views.py`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/sequence/models.py` & `accrete-0.0.9/accrete/contrib/sequence/models.py`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/sequence/queries.py` & `accrete-0.0.9/accrete/contrib/sequence/queries.py`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/sequence/migrations/0001_initial.py` & `accrete-0.0.9/accrete/contrib/sequence/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/system_mail/forms.py` & `accrete-0.0.9/accrete/contrib/system_mail/forms.py`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/system_mail/models.py` & `accrete-0.0.9/accrete/contrib/system_mail/models.py`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/system_mail/tasks.py` & `accrete-0.0.9/accrete/contrib/system_mail/tasks.py`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/system_mail/migrations/0001_initial.py` & `accrete-0.0.9/accrete/contrib/system_mail/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/ui/filter.py` & `accrete-0.0.9/accrete/contrib/ui/filter.py`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/ui/helper.py` & `accrete-0.0.9/accrete/contrib/ui/helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 ACTIONS_TEMPLATE = config.ACCRETE_UI_ACTIONS_TEMPLATE
 
 
 @dataclass
 class ClientAction:
 
     name: str
-    url: str = None
+    url: str = ''
+    query_params: str = ''
+    attrs: list[str] = field(default_factory=list)
     submit: bool = False
     form_id: str = 'form'
     class_list: list = field(default_factory=list)
     mobile: bool = True
     tablet: bool = True
 
 
@@ -37,15 +39,15 @@
     }
 
 
 @dataclass
 class BreadCrumb:
 
     name: str
-    url:str
+    url: str
 
 
 @dataclass
 class ListContext:
 
     model: type[Model]
     get_params: dict
@@ -344,35 +346,16 @@
 
 
 def get_related_model(model, path):
     related_model = model
     for part in path:
         try:
             related_model = related_model._meta.fields_map[part].related_model
-            continue
         except (AttributeError, KeyError):
-            pass
-        # try:
-        #     related_model = getattr(related_model, part).model
-        #     continue
-        # except AttributeError:
-        #     pass
-        # try:
-        #     related_model = getattr(related_model.rel.related_model, part)
-        #     continue
-        # except AttributeError:
-        #     pass
-        # try:
-        #     related_model = getattr(related_model, part).field.related_model
-        #     continue
-        # except AttributeError:
-        #     pass
-        raise AttributeError(
-            f'Could not resolve relation for model: {model} with path "{path}" at {part}'
-        )
+            continue
     return related_model
 
 
 def get_query(model, param: str, value) -> Q:
     invert = False
     parts = param.split('__')
     if param.startswith('~'):
```

### Comparing `accrete-0.0.8/accrete/contrib/ui/static/css/accrete.css` & `accrete-0.0.9/accrete/contrib/ui/static/css/accrete.css`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/ui/static/css/icons.css` & `accrete-0.0.9/accrete/contrib/ui/static/css/icons.css`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/ui/static/icons/Logo.svg` & `accrete-0.0.9/accrete/contrib/ui/static/icons/Logo.svg`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/ui/static/icons/accrete.svg` & `accrete-0.0.9/accrete/contrib/ui/static/icons/accrete.svg`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/ui/static/js/filter.js` & `accrete-0.0.9/accrete/contrib/ui/static/js/filter.js`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/ui/static/js/list.js` & `accrete-0.0.9/accrete/contrib/ui/static/js/list.js`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/ui/templates/django/forms/widgets/file.html` & `accrete-0.0.9/accrete/contrib/ui/templates/django/forms/widgets/file.html`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/ui/templates/ui/detail.html` & `accrete-0.0.9/accrete/contrib/ui/templates/ui/detail.html`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/ui/templates/ui/layout.html` & `accrete-0.0.9/accrete/contrib/ui/templates/ui/layout.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,114 +1,107 @@
 <!doctype html>
 {% load static %}
 {% load i18n %}
-{% load cache %}
+{% load accrete_ui %}
 
 <html lang="en">
+
 <head>
-    {% block head %}
-        <meta charset="utf-8">
-        <meta name="viewport" content="width=device-width, initial-scale=1">
-        {% block favicon %}
-            <link rel="icon" type="image/svg" href="{% static 'icons/accrete.svg' %}"/>
-        {% endblock %}
-        {% block bulma %}
-            <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bulma@0.9.4/css/bulma.min.css">
-        {% endblock %}
-        {% block style %}
-            <link rel="stylesheet" type="text/css" href="{% static "css/accrete.css" %}">
-            <link rel="stylesheet" type="text/css" href="{% static "css/icons.css" %}">
-        {% endblock %}
-        {% block htmx %}
-            <script src="https://unpkg.com/htmx.org@1.9.6"></script>
-            <script src="https://unpkg.com/hyperscript.org@0.9.11"></script>
-        {% endblock %}
-        {% block script %}
-            <script src="{% static "js/navbar.js" %}" defer type="text/javascript"></script>
-            <script src="{% static "js/utils.js" %}" defer type="text/javascript"></script>
-        {% endblock %}
+{% block head %}
+    <meta charset="utf-8">
+    <meta name="viewport" content="width=device-width, initial-scale=1">
+    {% block favicon %}<link rel="icon" type="image/svg" href="{% static 'icons/accrete.svg' %}"/>{% endblock %}
+    {% block bulma %}<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bulma@0.9.4/css/bulma.min.css">{% endblock %}
+    {% block style %}
+        <link rel="stylesheet" type="text/css" href="{% static "css/accrete.css" %}">
+        <link rel="stylesheet" type="text/css" href="{% static "css/icons.css" %}">
     {% endblock %}
-    {% block title_tag %}
-        <title>{% block title %}{{ title }}{% endblock %}</title>
+    {% block htmx %}
+        <script src="https://unpkg.com/htmx.org@1.9.6"></script>
+        <script src="https://unpkg.com/hyperscript.org@0.9.11"></script>
     {% endblock %}
+    {% block script %}
+        <script src="{% static "js/navbar.js" %}" defer type="text/javascript"></script>
+        <script src="{% static "js/utils.js" %}" defer type="text/javascript"></script>
+    {% endblock %}
+    <title>{% block title %}{{ title }}{% endblock %}</title>
+{% endblock %}
 </head>
 
-<body id="body" {% block body_attrs %}hx-headers='{"X-CSRFToken": "{{ csrf_token }}"}'{% endblock %}>
-    <nav id="navbar" class="navbar is-success is-info is-fixed-top" role="navigation" aria-label="main navigation">
-        <div class="navbar-brand">
-            {% block navbar_brand %}
-                {% if request.tenant %}
-                    <p class="navbar-item is-unselectable">
-                        {{ request.tenant.name }}
-                    </p>
-                {% endif %}
-                {% block navbar_brand_inside %}{% endblock %}
-                <a id="navbar-burger" role="button" class="navbar-burger accrete-burger"
-                   aria-label="menu" aria-expanded="false">
+
+<body {% block body_attrs %}hx-headers='{"X-CSRFToken": "{{ csrf_token }}"}'{% endblock %}>
+    {% block navbar %}
+        <nav id="navbar" class="navbar is-success is-fixed-top" role="navigation" aria-label="main navigation">
+            <div class="navbar-brand">
+                {% block navbar_brand %}
+                    <div class="navbar-item is-unselectable">{{ request.tenant.name }}</div>
+                {% endblock %}
+                <a id="navbar-burger" role="button" class="navbar-burger"
+                   aria-label="menu" aria-expanded="false"
+                   _="on click toggle .is-active on me then toggle .is-active on .navbar-menu"
+                >
                     {# Display hamburger menu on mobile #}
                     <span aria-hidden="true"></span>
                     <span aria-hidden="true"></span>
                     <span aria-hidden="true"></span>
                 </a>
-            {% endblock %}
-        </div>
-
-        <div class="navbar-menu is-fixed-top accrete-burger">
-            <div class="navbar-start">
-                {% block navbar_start %}
-                {% endblock %}
             </div>
 
-            <div class="navbar-end">
-                <div class="navbar-item has-dropdown accrete-navbar-menu">
+            <div class="navbar-menu is-fixed-top">
+                <div class="navbar-start">
+                    {% block navbar_start %}
+                        {% combine_templates 'accrete_menu.html' %}
+                    {% endblock %}
+                </div>
+
+                <div class="navbar-end">
                     {% block navbar_end %}
                     {% endblock %}
                 </div>
             </div>
-        </div>
-    </nav>
+        </nav>
+    {% endblock %}
 
     <div class="main-columns columns m-0 is-mobile">
         {% block main_columns %}
-            <div class="side-panel column is-3-widescreen is-2-fullhd is-hidden-touch is-hidden-desktop-only is-hidden-widescreen-only" style="height: 100%">
-                <nav class="panel is-shadowless pb-5">
-                    {% if list_pagination %}
-                        <div class="panel-block">
-                            {% include 'ui/partials/pagination_list.html' %}
-                        </div>
-                    {% endif %}
-                    {% if detail_pagination %}
-                        <div class="panel-block">
-                            {% include 'ui/partials/pagination_detail.html' %}
-                        </div>
-                    {% endif %}
-                    <div id="panel-actions">
-                        {% block side_panel_items %}{% if actions and actions_template %}{% include actions_template with all=True %}{% endif %}{% endblock %}
-                    </div>
-                    {% if filter_terms %}
-                        <div class="panel-list px-3 has-text-centered">
-                            <span>{% translate 'Filter' %}</span>
+            {% block side_panel %}
+                <div class="side-panel column is-3-widescreen is-2-fullhd is-hidden-touch is-hidden-desktop-only is-hidden-widescreen-only" style="height: 100%">
+                    <nav class="panel is-shadowless pb-5">
+                        {% if list_pagination %}
+                            <div class="panel-block">
+                                {% include 'ui/partials/pagination_list.html' %}
+                            </div>
+                        {% endif %}
+                        {% if detail_pagination %}
+                            <div class="panel-block">
+                                {% include 'ui/partials/pagination_detail.html' %}
+                            </div>
+                        {% endif %}
+                        <div id="panel-actions">
+                            {% block side_panel_items %}{% if actions and actions_template %}{% include actions_template with all=True %}{% endif %}{% endblock %}
                         </div>
-                        <div class="panel-block" style="position: sticky">
-                            <button id="reset-filter-button"
-                                    class="button is-fullwidth mr-1">{% translate 'Reset' %}
-                            </button>
-                            <button id="apply-filter-button"
-                                    class="button is-fullwidth ml-1">{% translate 'Filter' %}
-                            </button>
-                        </div>
-                        <div id="filter-panel">
-                            {% cache 500 filter_panel request.path request.GET request.tenant %}
+                        {% if filter_terms %}
+                            <div class="panel-list px-3 has-text-centered">
+                                <span>{% translate 'Filter' %}</span>
+                            </div>
+                            <div class="panel-block" style="position: sticky">
+                                <button id="reset-filter-button"
+                                        class="button is-fullwidth mr-1">{% translate 'Reset' %}
+                                </button>
+                                <button id="apply-filter-button"
+                                        class="button is-fullwidth ml-1">{% translate 'Filter' %}
+                                </button>
+                            </div>
+                            <div id="filter-panel">
                                 {% include 'ui/partials/filter.html' %}
-                            {% endcache %}
-                        </div>
-                    {% endif %}
-                </nav>
-            </div>
-
+                            </div>
+                        {% endif %}
+                    </nav>
+                </div>
+            {% endblock %}
 
             <div id="content" class="column content-column p-0" style="height: 100%; overflow-y: auto">
                 {% block content %}{% endblock %}
             </div>
         {% endblock %}
     </div>
```

#### html2text {}

```diff
@@ -1,41 +1,42 @@
-{% load static %} {% load i18n %} {% load cache %}
+{% load static %} {% load i18n %} {% load accrete_ui %}
 {% block head %}
 {% block favicon %}
 {% endblock %} {% block bulma %}
 {% endblock %} {% block style %}
 }">
 }"> {% endblock %} {% block htmx %}
 {% endblock %} {% block script %}
 }" defer type="text/javascript">
 }" defer type="text/javascript">
-{% endblock %} {% endblock %} {% block title_tag %}
+{% endblock %}
 {% endblock %}
 % block body_attrs %}hx-headers='{"X-CSRFToken": "{{ csrf_token }}"}'{%
-endblock %}>
-{% block navbar_brand %} {% if request.tenant %}
+endblock %}> {% block navbar %}
+{% block navbar_brand %}
 {{ request.tenant.name }}
-{% endif %} {% block navbar_brand_inside %}{% endblock %} {# Display hamburger
-menu on mobile #} {% endblock %}
-{% block navbar_start %} {% endblock %}
+{% endblock %} {# Display hamburger menu on mobile #}
+{% block navbar_start %} {% combine_templates 'accrete_menu.html' %} {%
+endblock %}
 {% block navbar_end %} {% endblock %}
-{% block main_columns %}
+{% endblock %}
+{% block main_columns %} {% block side_panel %}
 {% if list_pagination %}
 {% include 'ui/partials/pagination_list.html' %}
 {% endif %} {% if detail_pagination %}
 {% include 'ui/partials/pagination_detail.html' %}
 {% endif %}
 {% block side_panel_items %}{% if actions and actions_template %}{% include
 actions_template with all=True %}{% endif %}{% endblock %}
 {% if filter_terms %}
 {% translate 'Filter' %}
 {% translate 'Reset' %} {% translate 'Filter' %}
-{% cache 500 filter_panel request.path request.GET request.tenant %} {% include
-'ui/partials/filter.html' %} {% endcache %}
+{% include 'ui/partials/filter.html' %}
 {% endif %}
+{% endblock %}
 {% block content %}{% endblock %}
 {% endblock %}
 {% if filter_terms %}
 {% block search_modal_title %}{% translate 'Filter' %}{% endblock %}
 {% translate 'Reset' %} {% translate 'Filter' %}
 {% endif %} {% if actions %}
 {% block action_modal_title %}{% translate 'Actions' %}{% endblock %}
```

### Comparing `accrete-0.0.8/accrete/contrib/ui/templates/ui/list.html` & `accrete-0.0.9/accrete/contrib/ui/templates/ui/list.html`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/ui/templates/ui/table.html` & `accrete-0.0.9/accrete/contrib/ui/templates/ui/table.html`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/ui/templates/ui/partials/actions.html` & `accrete-0.0.9/accrete/contrib/ui/templates/ui/partials/actions.html`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,16 @@
                 {% if action.submit %}
                     <input class="button is-fullwidth {{ action.class_list|join:' ' }}"
                            type="submit" form={{ action.form_id }} value="{{ action.name }}"
                            style="white-space: normal; height: auto"
                            {{ action.attrs|join:' ' }}>
                 {% else %}
                 <a class="button is-fullwidth {{ action.class|join:' ' }}"
-                   href="{{ action.url }}{{ querystring }}{% if page %}&page={{ page.number }}{% endif %}" {{ action.attrs }}
+                   href="{{ action.url }}{{ querystring|default_if_none:'?' }}{% if page %}&page={{ page.number }}{% endif %}{{ action.query_params }}"
+                   {% for attr in action.attrs %}{{ attr }}{% endfor %}
                    style="word-break: break-word">{{ action.name }}
                 </a>
                 {% endif %}
             {% endif %}
         </div>
     {% endif %}
 {% endfor %}
```

### Comparing `accrete-0.0.8/accrete/contrib/ui/templates/ui/partials/filter.html` & `accrete-0.0.9/accrete/contrib/ui/templates/ui/partials/filter.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 {% load i18n %}
 {% load static %}
+{% load cache %}
 {% load accrete_ui %}
 
 <div id="query-block" class="panel-block pt-0" style="position: relative; display: inline-block; width: 100%">
     <div id="query-tags" class="is-flex-direction-column is-flex-grow-1 is-multiline mb-1" data-or-label="{% translate 'OR' %}"></div>
 
     <div class="field has-addons level">
         <p id="query-operation" class="control">
@@ -32,13 +33,12 @@
             </span>
         </p>
         <p id="query-input-apply" class="control"><button class="button">&#x21D2;</button></p>
     </div>
 
 
     <div id="query-params-dropdown" class="box mt-1 mx-0 p-1 is-hidden" tabindex="-1" style="z-index: 10; background: white; word-break: break-word; position: inherit">
-        {% for term in filter_terms %}
-
-        {% endfor %}
-        {{ filter_terms|render_query_params|safe }}
+        {% cache 500 filter_params request.path request.GET request.tenant %}
+            {{ filter_terms|render_query_params|safe }}
+        {% endcache %}
     </div>
 </div>
```

### Comparing `accrete-0.0.8/accrete/contrib/ui/templates/ui/partials/form_errors.html` & `accrete-0.0.9/accrete/contrib/ui/templates/ui/partials/form_errors.html`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/ui/templates/ui/partials/form_modal.html` & `accrete-0.0.9/accrete/contrib/ui/templates/ui/partials/form_modal.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,8 @@
             {% block modal_content %}{% endblock %}
         </section>
         <footer class="modal-card-foot">
             <input class="button is-success" type="submit" form="{{ form_id }}" value="{% translate 'Save' %}">
             <button class="button" hx-get="{% url 'ui:form_modal' %}" hx-swap="outerHTML" hx-target="#form-modal">{% translate 'Discard' %}</button>
         </footer>
     </div>
-</div>
+</div>
```

### Comparing `accrete-0.0.8/accrete/contrib/ui/templates/ui/partials/header.html` & `accrete-0.0.9/accrete/contrib/ui/templates/ui/partials/header.html`

 * *Files 2% similar despite different names*

```diff
@@ -62,129 +62,130 @@
 000003d0: 7264 223e 0a20 2020 2020 2020 2020 2020  rd">.           
 000003e0: 2020 2020 2020 2020 203c 756c 3e0a 2020           <ul>.  
 000003f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000400: 2020 2020 2020 7b25 2066 6f72 2063 7275        {% for cru
 00000410: 6d62 2069 6e20 6272 6561 6463 7275 6d62  mb in breadcrumb
 00000420: 7320 257d 0a20 2020 2020 2020 2020 2020  s %}.           
 00000430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000440: 203c 6c69 3e3c 6120 6872 6566 3d22 7b7b   <li><a href="{{
-00000450: 2063 7275 6d62 2e75 726c 7c64 6566 6175   crumb.url|defau
-00000460: 6c74 5f69 665f 6e6f 6e65 3a27 2327 207d  lt_if_none:'#' }
-00000470: 7d7b 7b20 7175 6572 7973 7472 696e 6720  }{{ querystring 
-00000480: 7d7d 2220 6172 6961 2d63 7572 7265 6e74  }}" aria-current
-00000490: 3d22 7061 6765 223e 7b7b 2063 7275 6d62  ="page">{{ crumb
-000004a0: 2e6e 616d 6520 7d7d 3c2f 613e 3c2f 6c69  .name }}</a></li
-000004b0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000004c0: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
-000004d0: 666f 7220 257d 0a20 2020 2020 2020 2020  for %}.         
-000004e0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000004f0: 6c69 2063 6c61 7373 3d22 6973 2d61 6374  li class="is-act
-00000500: 6976 6522 3e3c 6120 6172 6961 2d63 7572  ive"><a aria-cur
-00000510: 7265 6e74 3d22 7061 6765 223e 7b7b 2074  rent="page">{{ t
-00000520: 6974 6c65 207d 7d3c 2f61 3e3c 2f6c 693e  itle }}</a></li>
-00000530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000540: 2020 2020 203c 2f75 6c3e 0a20 2020 2020       </ul>.     
-00000550: 2020 2020 2020 2020 2020 203c 2f6e 6176             </nav
-00000560: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
-00000570: 6469 763e 0a20 2020 2020 2020 203c 2f64  div>.        </d
-00000580: 6976 3e0a 2020 2020 2020 2020 7b25 2069  iv>.        {% i
-00000590: 6620 6c69 7374 5f70 6167 696e 6174 696f  f list_paginatio
-000005a0: 6e20 6f72 2064 6574 6169 6c5f 7061 6769  n or detail_pagi
-000005b0: 6e61 7469 6f6e 2025 7d0a 2020 2020 2020  nation %}.      
-000005c0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-000005d0: 3d22 6c65 7665 6c2d 7269 6768 7420 6973  ="level-right is
-000005e0: 2d6d 6f62 696c 6520 6973 2d68 6964 6465  -mobile is-hidde
-000005f0: 6e2d 6d6f 6269 6c65 2069 732d 6869 6464  n-mobile is-hidd
-00000600: 656e 2d66 756c 6c68 6420 7078 2d33 206d  en-fullhd px-3 m
-00000610: 622d 3120 6973 2d61 6c69 676e 2d73 656c  b-1 is-align-sel
-00000620: 662d 666c 6578 2d73 7461 7274 223e 0a20  f-flex-start">. 
-00000630: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000640: 6469 7620 636c 6173 733d 226c 6576 656c  div class="level
-00000650: 2d69 7465 6d22 3e0a 2020 2020 2020 2020  -item">.        
-00000660: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
-00000670: 6620 6c69 7374 5f70 6167 696e 6174 696f  f list_paginatio
-00000680: 6e20 257d 0a20 2020 2020 2020 2020 2020  n %}.           
-00000690: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-000006a0: 696e 636c 7564 6520 2775 692f 7061 7274  include 'ui/part
-000006b0: 6961 6c73 2f70 6167 696e 6174 696f 6e5f  ials/pagination_
-000006c0: 6c69 7374 2e68 746d 6c27 2025 7d0a 2020  list.html' %}.  
-000006d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006e0: 2020 7b25 2065 6c69 6620 6465 7461 696c    {% elif detail
-000006f0: 5f70 6167 696e 6174 696f 6e20 257d 0a20  _pagination %}. 
-00000700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000710: 2020 2020 2020 207b 2520 696e 636c 7564         {% includ
-00000720: 6520 2775 692f 7061 7274 6961 6c73 2f70  e 'ui/partials/p
-00000730: 6167 696e 6174 696f 6e5f 6465 7461 696c  agination_detail
-00000740: 2e68 746d 6c27 2025 7d0a 2020 2020 2020  .html' %}.      
-00000750: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00000760: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
-00000770: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-00000780: 0a20 2020 2020 2020 2020 2020 203c 2f64  .            </d
-00000790: 6976 3e0a 2020 2020 2020 2020 7b25 2065  iv>.        {% e
-000007a0: 6e64 6966 2025 7d0a 2020 2020 3c2f 6469  ndif %}.    </di
-000007b0: 763e 0a0a 2020 2020 3c64 6976 2063 6c61  v>..    <div cla
-000007c0: 7373 3d22 6c65 7665 6c20 702d 3020 6d2d  ss="level p-0 m-
-000007d0: 3020 6973 2d6d 6f62 696c 6522 3e0a 2020  0 is-mobile">.  
-000007e0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-000007f0: 3d22 6c65 7665 6c2d 6c65 6674 223e 0a20  ="level-left">. 
-00000800: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00000810: 636c 6173 733d 226c 6576 656c 2d69 7465  class="level-ite
-00000820: 6d20 6973 2d6d 6f62 696c 6520 6973 2d68  m is-mobile is-h
-00000830: 6964 6465 6e2d 7461 626c 6574 206d 722d  idden-tablet mr-
-00000840: 3022 3e0a 2020 2020 2020 2020 2020 2020  0">.            
-00000850: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00000860: 6275 7474 6f6e 7322 3e0a 2020 2020 2020  buttons">.      
-00000870: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00000880: 2062 6c6f 636b 206d 6f62 696c 655f 6163   block mobile_ac
-00000890: 7469 6f6e 7320 257d 0a20 2020 2020 2020  tions %}.       
-000008a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008b0: 207b 2520 6966 2061 6374 696f 6e73 5f74   {% if actions_t
-000008c0: 656d 706c 6174 6520 257d 7b25 2069 6e63  emplate %}{% inc
-000008d0: 6c75 6465 2061 6374 696f 6e73 5f74 656d  lude actions_tem
-000008e0: 706c 6174 6520 7769 7468 206d 6f62 696c  plate with mobil
-000008f0: 653d 5472 7565 2025 7d7b 2520 656e 6469  e=True %}{% endi
-00000900: 6620 257d 0a20 2020 2020 2020 2020 2020  f %}.           
-00000910: 2020 2020 2020 2020 207b 2520 656e 6462           {% endb
-00000920: 6c6f 636b 2025 7d0a 2020 2020 2020 2020  lock %}.        
-00000930: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-00000940: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
-00000950: 3e0a 0a20 2020 2020 2020 2020 2020 203c  >..            <
-00000960: 6469 7620 636c 6173 733d 226c 6576 656c  div class="level
-00000970: 2d69 7465 6d20 6973 2d6d 6f62 696c 6520  -item is-mobile 
-00000980: 6973 2d68 6964 6465 6e2d 6675 6c6c 6864  is-hidden-fullhd
-00000990: 2069 732d 6869 6464 656e 2d6d 6f62 696c   is-hidden-mobil
-000009a0: 6520 6d72 2d30 223e 0a20 2020 2020 2020  e mr-0">.       
-000009b0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-000009c0: 6173 733d 2262 7574 746f 6e73 223e 0a20  ass="buttons">. 
-000009d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009e0: 2020 207b 2520 626c 6f63 6b20 7461 626c     {% block tabl
-000009f0: 6574 5f61 6374 696f 6e73 2025 7d0a 2020  et_actions %}.  
-00000a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a10: 2020 2020 2020 7b25 2069 6620 6163 7469        {% if acti
-00000a20: 6f6e 735f 7465 6d70 6c61 7465 2025 7d7b  ons_template %}{
-00000a30: 2520 696e 636c 7564 6520 6163 7469 6f6e  % include action
-00000a40: 735f 7465 6d70 6c61 7465 2077 6974 6820  s_template with 
-00000a50: 7461 626c 6574 3d54 7275 6520 257d 7b25  tablet=True %}{%
-00000a60: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
-00000a70: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00000a80: 2065 6e64 626c 6f63 6b20 257d 0a20 2020   endblock %}.   
-00000a90: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-00000aa0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-00000ab0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-00000ac0: 2020 203c 6469 7620 636c 6173 733d 226c     <div class="l
-00000ad0: 6576 656c 2d69 7465 6d20 6973 2d6d 6f62  evel-item is-mob
-00000ae0: 696c 6520 6973 2d68 6964 6465 6e2d 6675  ile is-hidden-fu
-00000af0: 6c6c 6864 2069 732d 6869 6464 656e 2d6d  llhd is-hidden-m
-00000b00: 6f62 696c 6520 6d72 2d30 223e 0a20 2020  obile mr-0">.   
-00000b10: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-00000b20: 7620 636c 6173 733d 2262 7574 746f 6e73  v class="buttons
-00000b30: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00000b40: 2020 2020 2020 203c 6275 7474 6f6e 2069         <button i
-00000b50: 643d 226d 6f64 616c 2d66 696c 7465 722d  d="modal-filter-
-00000b60: 6275 7474 6f6e 2220 636c 6173 733d 2262  button" class="b
-00000b70: 7574 746f 6e22 3e46 696c 7465 723c 2f62  utton">Filter</b
-00000b80: 7574 746f 6e3e 0a20 2020 2020 2020 2020  utton>.         
-00000b90: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-00000ba0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-00000bb0: 0a20 2020 2020 2020 203c 2f64 6976 3e0a  .        </div>.
-00000bc0: 2020 2020 3c2f 6469 763e 0a3c 2f64 6976      </div>.</div
-00000bd0: 3e                                       >
+00000440: 203c 6c69 3e3c 6120 636c 6173 733d 2269   <li><a class="i
+00000450: 732d 756e 6465 726c 696e 6564 2220 6872  s-underlined" hr
+00000460: 6566 3d22 7b7b 2063 7275 6d62 2e75 726c  ef="{{ crumb.url
+00000470: 7c64 6566 6175 6c74 5f69 665f 6e6f 6e65  |default_if_none
+00000480: 3a27 2327 207d 7d7b 7b20 7175 6572 7973  :'#' }}{{ querys
+00000490: 7472 696e 6720 7d7d 2220 6172 6961 2d63  tring }}" aria-c
+000004a0: 7572 7265 6e74 3d22 7061 6765 223e 7b7b  urrent="page">{{
+000004b0: 2063 7275 6d62 2e6e 616d 6520 7d7d 3c2f   crumb.name }}</
+000004c0: 613e 3c2f 6c69 3e0a 2020 2020 2020 2020  a></li>.        
+000004d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000004e0: 7b25 2065 6e64 666f 7220 257d 0a20 2020  {% endfor %}.   
+000004f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000500: 2020 2020 203c 6c69 2063 6c61 7373 3d22       <li class="
+00000510: 6973 2d61 6374 6976 6522 3e3c 6120 6172  is-active"><a ar
+00000520: 6961 2d63 7572 7265 6e74 3d22 7061 6765  ia-current="page
+00000530: 223e 7b7b 2074 6974 6c65 207d 7d3c 2f61  ">{{ title }}</a
+00000540: 3e3c 2f6c 693e 0a20 2020 2020 2020 2020  ></li>.         
+00000550: 2020 2020 2020 2020 2020 203c 2f75 6c3e             </ul>
+00000560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000570: 203c 2f6e 6176 3e0a 2020 2020 2020 2020   </nav>.        
+00000580: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
+00000590: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+000005a0: 2020 7b25 2069 6620 6c69 7374 5f70 6167    {% if list_pag
+000005b0: 696e 6174 696f 6e20 6f72 2064 6574 6169  ination or detai
+000005c0: 6c5f 7061 6769 6e61 7469 6f6e 2025 7d0a  l_pagination %}.
+000005d0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+000005e0: 2063 6c61 7373 3d22 6c65 7665 6c2d 7269   class="level-ri
+000005f0: 6768 7420 6973 2d6d 6f62 696c 6520 6973  ght is-mobile is
+00000600: 2d68 6964 6465 6e2d 6d6f 6269 6c65 2069  -hidden-mobile i
+00000610: 732d 6869 6464 656e 2d66 756c 6c68 6420  s-hidden-fullhd 
+00000620: 7078 2d33 206d 622d 3120 6973 2d61 6c69  px-3 mb-1 is-ali
+00000630: 676e 2d73 656c 662d 666c 6578 2d73 7461  gn-self-flex-sta
+00000640: 7274 223e 0a20 2020 2020 2020 2020 2020  rt">.           
+00000650: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00000660: 226c 6576 656c 2d69 7465 6d22 3e0a 2020  "level-item">.  
+00000670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000680: 2020 7b25 2069 6620 6c69 7374 5f70 6167    {% if list_pag
+00000690: 696e 6174 696f 6e20 257d 0a20 2020 2020  ination %}.     
+000006a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006b0: 2020 207b 2520 696e 636c 7564 6520 2775     {% include 'u
+000006c0: 692f 7061 7274 6961 6c73 2f70 6167 696e  i/partials/pagin
+000006d0: 6174 696f 6e5f 6c69 7374 2e68 746d 6c27  ation_list.html'
+000006e0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+000006f0: 2020 2020 2020 2020 7b25 2065 6c69 6620          {% elif 
+00000700: 6465 7461 696c 5f70 6167 696e 6174 696f  detail_paginatio
+00000710: 6e20 257d 0a20 2020 2020 2020 2020 2020  n %}.           
+00000720: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+00000730: 696e 636c 7564 6520 2775 692f 7061 7274  include 'ui/part
+00000740: 6961 6c73 2f70 6167 696e 6174 696f 6e5f  ials/pagination_
+00000750: 6465 7461 696c 2e68 746d 6c27 2025 7d0a  detail.html' %}.
+00000760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000770: 2020 2020 7b25 2065 6e64 6966 2025 7d0a      {% endif %}.
+00000780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000790: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+000007a0: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+000007b0: 2020 7b25 2065 6e64 6966 2025 7d0a 2020    {% endif %}.  
+000007c0: 2020 3c2f 6469 763e 0a0a 2020 2020 3c64    </div>..    <d
+000007d0: 6976 2063 6c61 7373 3d22 6c65 7665 6c20  iv class="level 
+000007e0: 702d 3020 6d2d 3020 6973 2d6d 6f62 696c  p-0 m-0 is-mobil
+000007f0: 6522 3e0a 2020 2020 2020 2020 3c64 6976  e">.        <div
+00000800: 2063 6c61 7373 3d22 6c65 7665 6c2d 6c65   class="level-le
+00000810: 6674 223e 0a20 2020 2020 2020 2020 2020  ft">.           
+00000820: 203c 6469 7620 636c 6173 733d 226c 6576   <div class="lev
+00000830: 656c 2d69 7465 6d20 6973 2d6d 6f62 696c  el-item is-mobil
+00000840: 6520 6973 2d68 6964 6465 6e2d 7461 626c  e is-hidden-tabl
+00000850: 6574 206d 722d 3022 3e0a 2020 2020 2020  et mr-0">.      
+00000860: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00000870: 6c61 7373 3d22 6275 7474 6f6e 7322 3e0a  lass="buttons">.
+00000880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000890: 2020 2020 7b25 2062 6c6f 636b 206d 6f62      {% block mob
+000008a0: 696c 655f 6163 7469 6f6e 7320 257d 0a20  ile_actions %}. 
+000008b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008c0: 2020 2020 2020 207b 2520 6966 2061 6374         {% if act
+000008d0: 696f 6e73 5f74 656d 706c 6174 6520 257d  ions_template %}
+000008e0: 7b25 2069 6e63 6c75 6465 2061 6374 696f  {% include actio
+000008f0: 6e73 5f74 656d 706c 6174 6520 7769 7468  ns_template with
+00000900: 206d 6f62 696c 653d 5472 7565 2025 7d7b   mobile=True %}{
+00000910: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
+00000920: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00000930: 2520 656e 6462 6c6f 636b 2025 7d0a 2020  % endblock %}.  
+00000940: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00000950: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00000960: 203c 2f64 6976 3e0a 0a20 2020 2020 2020   </div>..       
+00000970: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00000980: 226c 6576 656c 2d69 7465 6d20 6973 2d6d  "level-item is-m
+00000990: 6f62 696c 6520 6973 2d68 6964 6465 6e2d  obile is-hidden-
+000009a0: 6675 6c6c 6864 2069 732d 6869 6464 656e  fullhd is-hidden
+000009b0: 2d6d 6f62 696c 6520 6d72 2d30 223e 0a20  -mobile mr-0">. 
+000009c0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000009d0: 6469 7620 636c 6173 733d 2262 7574 746f  div class="butto
+000009e0: 6e73 223e 0a20 2020 2020 2020 2020 2020  ns">.           
+000009f0: 2020 2020 2020 2020 207b 2520 626c 6f63           {% bloc
+00000a00: 6b20 7461 626c 6574 5f61 6374 696f 6e73  k tablet_actions
+00000a10: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00000a20: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
+00000a30: 6620 6163 7469 6f6e 735f 7465 6d70 6c61  f actions_templa
+00000a40: 7465 2025 7d7b 2520 696e 636c 7564 6520  te %}{% include 
+00000a50: 6163 7469 6f6e 735f 7465 6d70 6c61 7465  actions_template
+00000a60: 2077 6974 6820 7461 626c 6574 3d54 7275   with tablet=Tru
+00000a70: 6520 257d 7b25 2065 6e64 6966 2025 7d0a  e %}{% endif %}.
+00000a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a90: 2020 2020 7b25 2065 6e64 626c 6f63 6b20      {% endblock 
+00000aa0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+00000ab0: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+00000ac0: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
+00000ad0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00000ae0: 6173 733d 226c 6576 656c 2d69 7465 6d20  ass="level-item 
+00000af0: 6973 2d6d 6f62 696c 6520 6973 2d68 6964  is-mobile is-hid
+00000b00: 6465 6e2d 6675 6c6c 6864 2069 732d 6869  den-fullhd is-hi
+00000b10: 6464 656e 2d6d 6f62 696c 6520 6d72 2d30  dden-mobile mr-0
+00000b20: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00000b30: 2020 203c 6469 7620 636c 6173 733d 2262     <div class="b
+00000b40: 7574 746f 6e73 223e 0a20 2020 2020 2020  uttons">.       
+00000b50: 2020 2020 2020 2020 2020 2020 203c 6275               <bu
+00000b60: 7474 6f6e 2069 643d 226d 6f64 616c 2d66  tton id="modal-f
+00000b70: 696c 7465 722d 6275 7474 6f6e 2220 636c  ilter-button" cl
+00000b80: 6173 733d 2262 7574 746f 6e22 3e46 696c  ass="button">Fil
+00000b90: 7465 723c 2f62 7574 746f 6e3e 0a20 2020  ter</button>.   
+00000ba0: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
+00000bb0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+00000bc0: 3c2f 6469 763e 0a20 2020 2020 2020 203c  </div>.        <
+00000bd0: 2f64 6976 3e0a 2020 2020 3c2f 6469 763e  /div>.    </div>
+00000be0: 0a3c 2f64 6976 3e                        .</div>
```

### Comparing `accrete-0.0.8/accrete/contrib/ui/templates/ui/partials/pagination_detail.html` & `accrete-0.0.9/accrete/contrib/ui/templates/ui/partials/pagination_detail.html`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/ui/templates/ui/partials/pagination_list.html` & `accrete-0.0.9/accrete/contrib/ui/templates/ui/partials/pagination_list.html`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/ui/templatetags/accrete_ui.py` & `accrete-0.0.9/accrete/contrib/ui/templatetags/accrete_ui.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,26 @@
 from django import template
+from django.conf import settings
+from django.template.loader import render_to_string
+from django.utils.safestring import mark_safe
 
 register = template.Library()
 
 
+@register.simple_tag(name='combine_templates')
+def combine_templates(template_name):
+    html = ''
+    for app in settings.INSTALLED_APPS:
+        try:
+            html += render_to_string(f'{app.split(".")[-1]}/{template_name}')
+        except template.TemplateDoesNotExist:
+            continue
+    return mark_safe(html)
+
+
 @register.filter(name='render_query_params')
 def query_params_to_html(params):
     html = ''
     for param in params:
         html += build(param)
     return html
```

### Comparing `accrete-0.0.8/accrete/contrib/user/models.py` & `accrete-0.0.9/accrete/contrib/user/models.py`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/user/views.py` & `accrete-0.0.9/accrete/contrib/user/views.py`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/user/locale/de/LC_MESSAGES/django.po` & `accrete-0.0.9/accrete/contrib/user/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/user/migrations/0001_initial.py` & `accrete-0.0.9/accrete/contrib/user/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/user/templates/user/login.html` & `accrete-0.0.9/accrete/contrib/user/templates/user/login.html`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/user_registration/forms.py` & `accrete-0.0.9/accrete/contrib/user_registration/forms.py`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/user_registration/views.py` & `accrete-0.0.9/accrete/contrib/user_registration/views.py`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/user_registration/migrations/0001_initial.py` & `accrete-0.0.9/accrete/contrib/user_registration/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/contrib/user_registration/templates/user_registration/registration.html` & `accrete-0.0.9/accrete/contrib/user_registration/templates/user_registration/registration.html`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/migrations/0001_initial.py` & `accrete-0.0.9/accrete/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/migrations/0002_initial.py` & `accrete-0.0.9/accrete/migrations/0002_initial.py`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/accrete/utils/dates.py` & `accrete-0.0.9/accrete/utils/dates.py`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/LICENSE` & `accrete-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/README.md` & `accrete-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `accrete-0.0.8/pyproject.toml` & `accrete-0.0.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ['hatchling']
 build-backend = 'hatchling.build'
 
 [project]
 name = 'accrete'
-version = '0.0.8'
+version = '0.0.9'
 authors = [
   { name='Benedikt Jilek', email='benedikt.jilek@pm.me' },
 ]
-description = 'Django Shared Schema Multi Tenant SaaS Foundation'
+description = 'Django Shared Schema Multi Tenant'
 readme = 'README.md'
 license = {file = 'LICENSE'}
 requires-python = '>=3.10'
 classifiers = [
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
@@ -34,13 +34,9 @@
 contrib = [
     'celery >= 5.3.4',
     'django_celery_beat'
 ]
 
 [tool.hatch.build]
 exclude = [
-    'project/',
-    '.idea/',
-    '.gitignore',
-    'manage.py',
-    'db.sqlite3'
+    '.git/'
 ]
```

### Comparing `accrete-0.0.8/PKG-INFO` & `accrete-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: accrete
-Version: 0.0.8
-Summary: Django Shared Schema Multi Tenant SaaS Foundation
+Version: 0.0.9
+Summary: Django Shared Schema Multi Tenant
 Author-email: Benedikt Jilek <benedikt.jilek@pm.me>
 License: Copyright (c) 2023 Benedikt Jilek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

